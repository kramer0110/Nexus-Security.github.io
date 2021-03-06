---
title: 'Go''s Tooling Is an Undervalued Technology'
date: 2020-01-22T03:53:00+01:00
draft: false
---

January 21, 2020

nullprogram.com/blog/2020/01/21/

Regardless of your opinions of the [Go programming language](https://golang.org/), the primary implementation of Go, gc, is an incredible piece of software engineering. Everyone ought to be blown away by it! Yet not only is it undervalued in general, even the Go community itself doesn’t fully appreciate it. It’s not perfect, but it has unique features never before seen in a toolchain.

In this article, when I say “Go” I’m referring to the gc compiler.

### Building Go

Since Go 1.5, Go is implemented in Go. It also has no external dependencies, so to build Go only a Go compiler is required. On my laptop, building the latest version of Go takes only 43 seconds. That includes the compiler, linker, all cross-compilers, and the standard library.

```
$ tar xzf go1.13.6.src.tar.gz $ cd go/src/ $ ./make.bash 
```

Cross-compiling Go — as in to build a Go toolchain for another platform supported by Go — only requires setting a couple of environment variables (`GOOS`, `GOARCH`). So, in a mere 43 seconds I can compile an _entire toolchain_ for _any supported host_! If you already have a Go compiler on your system, there’s no reason to bother with binary releases. Just grab the source and build it. All can manage their own toolchain with ease!

Anyone who’s ever built a GCC or Clang+LLVM toolchain, _especially_ anyone who’s built cross-compiler toolchains, should find this situation totally bonkers. How could it possibly be so easy and so fast? GCC’s configure script [wouldn’t even finish](https://nullprogram.com/blog/2017/03/30/) before Go was already built.

Yes, this comparison is a bit apples and oranges. Both GCC and LLVM are more advanced compilers and produce much more efficient code, so of course there’s more to them, and of course they take longer to build. But does that completely justify the difference? This goes double for GCC and LLVM cross-compiler toolchains, which are, for the most part, very complex and difficult to build.

If you don’t already have Go, all you need is a C compiler and the Go 1.4 source code. [Bootstrapping](https://nullprogram.com/blog/2016/11/17/) through Go 1.4 is easy, and I’ve done it a number of times. I keep a copy of the Go 1.4 tarball just for this reason.

How Go could improve: [The linker could be better](http://golang.org/s/better-linker). Binaries are already too big, and getting bigger with each release. This problem is acknowledged by the Go developers:

> The original linker was also simpler than it is now and its implementation fit in [one Turing award winner’s head](https://en.wikipedia.org/wiki/Ken_Thompson), so there’s little abstraction or modularity. Unfortunately, as the linker grew and evolved, it retained its lack of structure, and our sole Turing award winner retired.

The story for native interop (cgo) [isn’t great either](https://dave.cheney.net/2016/01/18/cgo-is-not-go) and requires trading away Go’s biggest strengths.

### Package Management

Go has decentralized package management — or, more accurately, _module_ management. There’s no central module manager or module registration. To use a Go module, it need only be hosted on a reachable network with a valid HTTPS certificate. Modules are named by a module path that includes its network location. This means there’s no land grab for [popular module names](https://github.com/dateutil/dateutil/issues/984).

An organization using Go does not need to trust an external package repository (PyPI, etc.), nor do they need to run an internal package repository for their own internal packages. In general it’s sufficient just to leverage the organization’s already-existing source control system.

Dependencies are locked to a particular version cryptographically. The upstream source cannot change a published module for those that already depend on it. They _could_ still publish a new version with [hostile changes](https://blog.npmjs.org/post/180565383195/details-about-the-event-stream-incident), but one should be cautious about updating dependencies — a deliberate action — [or even having dependencies in the first place](https://research.swtch.com/deps).

With decentralized module management, you might think that each dependency host is a single point of failure — and you would be exactly right. If any dependency disappears, you can no longer build in a fresh checkout. Go has a solution for this: a _module proxy_. Before fetching the dependency directly, Go (optionally, configured via `GOPROXY`) checks with a module proxy that may have cached the dependency. This eliminates the single point of failure. Google hosts a free module proxy service for the internet, but organizations should probably run their own module proxy internally, at least for external dependencies. This neatly solves [the left-pad problem](https://lwn.net/Articles/681410/).

Honestly, this is a breath of fresh air. Decentralized modules are great idea and avoid most of the issues of a centralized package repositories.

How Go could improve: Go’s module management is a little _too_ gung-ho about HTTPS and certificates. The module documentation is still incomplete, and the only way to get answers to some of my questions was either to find the relevant source code in Go or to simply experiment.

Normally I could experiment using my local system, but Go refuses to do anything with modules unless I go through HTTPS with valid certificates. Needing to do bunch of pointless configuration — creating a dummy CA, dummy localhost certificates, and setting it all up — really kills my momentum and motivation, and it delayed me in learning the new module system. Before modules, Go supported an `-insecure` flag, which was great for this sort of experimentation, but they removed it out of fear of misuse. I’ll decide my own risks, thank you very much.

An example of a question without a documented answer: If my module path is `example.com/foo` but my web server 301 redirects this request to `example.com/foo/`, will Go follow this redirect _and_ re-append `?go-get=1`? (Yes.) Did I want to configure an HTTPS server just to test this? (No.)

#### Vendoring

I still haven’t even gotten to one of the most powerful and unique module features — a feature which the Go developers initially didn’t want to include. If you have a `vendor/` directory at the root of your module, and you use `-mod=vendor` when compiling, Go will look in that directory for modules. Go’s build system before modules (`GOPATH`) had a similar mechanism.

This is called _vendoring_ and the practice pre-dates Go itself. Just check your dependency sources directly into source control alongside your own sources and hook them into your build. Organizations will often use this internally to lock down dependencies and to avoid depending on external resources. Typically, vendoring is a lot of work. The project’s build system must cooperate with the dependency’s build system. Then eventually you may want to update a vendored dependency, which may require more build changes.

These issues have led to the rise of [_header libraries_](https://github.com/nothings/stb) and [amalgamations](https://www.sqlite.org/amalgamation.html) in C and C++: libraries that are trivial to integrate into any project.

**Go’s module system fully automates vendoring**, which it can do because it already orchestrates builds. A single command populates the `vendor/` directory with all of the module’s current dependencies:

Normally you might follow this up by checking it into source control, but that’s not the only way it’s useful. Instead a project could merely include the `vendor/` directory in its release source tarball. That tarball would be the _entire_, standalone source for that release. With all external dependencies packed into the tarball, the program could be built entirely offline on any system with a Go compiler. This is incredibly useful for me personally.

Some open source projects _not_ written in Go have dependencies-included releases like this ([example](https://crawl.develz.org/)), but it’s a ton of work. So, of course, it’s usually not done. However, any Go project (not using cgo) can accomplish this _trivially_ without even thinking about it. This is a such big deal, and nobody’s talking about it!

There’s lots of discussion about Go the programming language, but I hardly see discussion about the amazing engineering that’s gone into Go itself. It’s an under-appreciated piece of technology!

  
  
from Hacker News https://ift.tt/2Ga7FXV