---
title: 'ICYMI CircuitPython Newsletter: CircuitPython is out of this world! Doc
Holliday stops by and
more! #Python #Adafruit #CircuitPython #PythonHardware #ICYMI @circuitpython @micropython @ThePSF @Adafruit'
date: 2019-09-25T14:38:00+01:00
draft: false
---

ICYMI (In case you missed it) – Tuesday’s Python on Microcontrollers Newsletter from [AdafruitDaily.com](https://www.adafruitdaily.com/) went out – if you missed it, [subscribe now!](https://www.adafruitdaily.com/)

The next newsletter goes out in a week and being subscribed the best way to keep up with all things Python for hardware.

Over 6k+ subscribers worldwide!

Max Holliday – CircuitPython in space, SmallSats and more!
==========================================================

[![Max in space](https://cdn-blog.adafruit.com/uploads/2019/09/92419space.jpg)](https://youtu.be/Mb9c4e7ID9E)

[Max Holliday](https://github.com/maholli) has been integrating CircuitPython into many aspects of his PhD research at Stanford University. We had a great time together chatting ([video](https://youtu.be/Mb9c4e7ID9E)). Thank you [Max](https://twitter.com/maholli404)! Topics included:

[![PyCubed](https://cdn-blog.adafruit.com/uploads/2019/09/92419pycubed.jpg)](http://pycubed.org/)

[KickSat-2](https://www.nasa.gov/ames/kicksat/) development yielded the [PyCubed project](http://pycubed.org/) and after Max’s talk at SmallSat 2019, over 60 universities have reached out wanting to use and/or incorporate PyCubed into their Cubesat development efforts.

[![KickSat](https://cdn-blog.adafruit.com/uploads/2019/03/python_in_space.gif)](https://www.nasa.gov/ames/kicksat/)

All of the radiation testing, data collection, etc. … for the research is collected using CircuitPython.

[![SX1280](https://cdn-blog.adafruit.com/uploads/2019/09/92419sx1280.jpg)](https://github.com/maholli/sx1280-breakout)

[![SX1280](https://cdn-blog.adafruit.com/uploads/2019/09/92419sx1280_on_adafruit.jpg)](https://github.com/maholli/sx1280-breakout)

Max is really excited lately with the time-of-flight ranging capability of the Semtech SX1280 radios. So Max [built a breakout](https://github.com/maholli/sx1280-breakout) that fits existing HopeRF footprints and published a working (albeit rough around the edges) [CircuitPython library](https://github.com/maholli/CircuitPython_SX1280)!

[![Keysight](https://cdn-blog.adafruit.com/uploads/2019/09/92419keysight.jpg)](https://www.iotchallengekeysight.com/)

Max was in NYC for this [Keysight IoT competition](https://www.iotchallengekeysight.com/). Using the KickSat-2 CircuitPython platform (the small form-factor sprites), Max’s team worked with a chemical engineering group at Stanford to develop a [completely new means of measuring ammonia concentrations in water](https://www.iotchallengekeysight.com/2019/entries/smart-water/257-0515-132058-immersible-internet-of-things-iot-sensors-for-cloud-based-water-quality-monitoring). The mesh network, gateways, sensing nodes, etc. are all using CircuitPython.

Max’s contributions to the Maker community and Stanford curriculum include:

[![SAM32](https://cdn-blog.adafruit.com/uploads/2019/09/92419sam32.jpg)](https://www.notion.so/SAM32-Guides-6b7e8ca318ff49418eec16e975d98f5d)

Max developed the [SAM32 board](https://www.notion.so/SAM32-Guides-6b7e8ca318ff49418eec16e975d98f5d) as a “catch-all” or swiss-army knife for student projects. It’s is now part the curriculum in 5+ courses in the fall.

[![MEMs](https://cdn-blog.adafruit.com/uploads/2019/09/92419e240.jpg)](https://www.notion.so/SAM32-Guides-6b7e8ca318ff49418eec16e975d98f5d)

One example, Eng240, is a MEMS course that’s historically been purely theory-based. However, Prof. Roger Howe and Max have overhauled the class to include labs in the fall. The first of which has students assembling their own SAM32, the second has students designing their own “marco” accelerometer using PCBs. Everything is driven with CircuitPython.

[![Soldering](https://cdn-blog.adafruit.com/uploads/2019/09/92419solder01.jpg)](https://sites.google.com/stanford.edu/soldering-internal/learning)

[![Soldering](https://cdn-blog.adafruit.com/uploads/2019/09/92419solder02.jpg)](https://sites.google.com/stanford.edu/soldering-internal/learning)

Max is a self described soldering nerd, and he was completely dissatisfied with resources online for folks learning to solder. [Max made a very polished tutorial](https://sites.google.com/stanford.edu/soldering-internal/learning) with a self-assessment quiz. Then he coupled it with a soldering practice + exam board for Stanford students to use.

Program CircuitPython devices with iPhone & iOS 13
--------------------------------------------------

[![CPiOS](https://cdn-blog.adafruit.com/uploads/2019/09/92419cirpy-plus-iphone-1.jpg)](https://blog.adafruit.com/2019/09/19/program-circuitpython-devices-with-iphone-ios-13/)

With the launch of iOS 13, iPhone users now have the ability to edit code on CircuitPython USB devices! Once you’re device is updated, you can connect a board such as Circuit Playground Express and edit & run code on the go – [Adafruit](https://blog.adafruit.com/2019/09/19/program-circuitpython-devices-with-iphone-ios-13/).

CircuitPython snakes its way to the FT232H
------------------------------------------

[![FT232H](https://cdn-blog.adafruit.com/uploads/2019/09/92419ft23h.jpg)](https://youtu.be/rriKd9jkdJQ)

The FT232H is a handy USB to GPIO/I2C/SPI breakout board we’ve stocked for a long time. It is used by lots of folks as a hardware interfacing bridge. For a long time, we’ve had Python support for it, but that support has gotten kind of old and neglected as we’ve spent a lot of our efforts on CircuitPython. Well, now we have CircuitPython Blinka support, so you can control sensors, OLEDs, buttons, LEDs and more all via FT232H! All thanks to Carter who fearlessly took on this code support – we’ll start writing up a guide in the next week or two – [YouTube](https://youtu.be/rriKd9jkdJQ).

CircuitPython slithers its way to Halloween! HackSpace issue 23!
----------------------------------------------------------------

[![Halloween HackSpace](https://cdn-blog.adafruit.com/uploads/2019/09/92419HackSpaceMagazine23.jpg)](https://hackspace.raspberrypi.org/issues/23)

[Issue 23 – HackSpace magazine: Halloween builds!](https://hackspace.raspberrypi.org/issues/23)

Turn to the fun (and dark) side of making with a look at the best crazy, creative Halloween builds around – then have a go at making your own! There are a lot of CircuitPython and Python projects in this issue, check it out and help support a great magazine!

[Read more](https://hackspace.raspberrypi.org/issues/23), [download PDF](https://magazines-static.raspberrypi.org/issues/full_pdfs/000/000/134/original/HackSpaceMagazine23.pdf?1568741893), [buy now](https://the-magpi-store.myshopify.com/admin/products/4022753362019), [subscribe](https://hackspace.raspberrypi.org/subscribe).

[![Subscribe](https://cdn-blog.adafruit.com/uploads/2019/09/92419HS_23_Subs.jpg)](https://hackspace.raspberrypi.org/subscribe)

[Subscribers](https://hackspace.raspberrypi.org/subscribe) save a bunch and they get a free Circuit Playground Express!

Send data with If This Then That – Control almost anything with CircuitPython
-----------------------------------------------------------------------------

[![IFTTT CircuitPython](https://cdn-blog.adafruit.com/uploads/2019/09/92419ifttcphs01.jpg)](https://hackspace.raspberrypi.org/issues/23)

[![IFTTT CircuitPython](https://cdn-blog.adafruit.com/uploads/2019/09/92419ifttcphs02.jpg)](https://hackspace.raspberrypi.org/issues/23)

[Issue 23 – HackSpace magazine: Send data with If This Then That – Control almost anything with CircuitPython by Ben Everard](https://hackspace.raspberrypi.org/issues/23) –

> _“If This Then That (IFTTT) is a really simple bit of glue that lets you link a condition with an action, both of which are taken from web services. All IFTTT applets are in the format If ‘condition’ then ‘action’. This simple form is surprisingly powerful because it’s linked to a huge number of internet services and web-connected devices. The sheer range of services that can link together, and the fact that everything can be configured by clicking on things in a website, make it a great platform for basic Internet of Things devices and experiments.”_

[Read more](https://hackspace.raspberrypi.org/issues/23) pages 78 to 81, [download PDF](https://magazines-static.raspberrypi.org/issues/full_pdfs/000/000/134/original/HackSpaceMagazine23.pdf?1568741893).

Motorized wing, making your cosplay move
----------------------------------------

[![Motorized wing](https://cdn-blog.adafruit.com/uploads/2019/09/92419motwingcphs01.jpg)](https://hackspace.raspberrypi.org/issues/23)

[![Motorized wing](https://cdn-blog.adafruit.com/uploads/2019/09/92419motwingcphs02.jpg)](https://hackspace.raspberrypi.org/issues/23)

[Issue 23 – HackSpace magazine: Motorized wing, making your cosplay move, add a servo for breathtaking effects](https://hackspace.raspberrypi.org/issues/23) by Sophy Wong –

> _“Add movement to your cosplay with a servo motor! In this intermediate build, we’ll make an articulating wing that opens and closes at the touch of a finger. This project is a perfect add-on to a sci-fi robot costume, a steampunk aviator, or any costume with a shoulder pauldron. We’ll bring our wing to life with some crafting, soldering, and a little bit of code! We’ve kept this build simple with everyday materials like cardboard and string. Clean, used shipping boxes are a great source of 4mm corrugated cardboard. A laser cutter makes quick work of cutting out the wings, but if you don’t have access to one, use scissors or a craft knife to cut the cardboard by hand. Our cyberpunk-style wing template includes design lines that can be engraved or traced on the surface of the wing for more texture. Download our template at [hsmag.cc/issue23](http://hsmag.cc/issue23), or create your own custom wing shape from scratch. Just make sure the pivoting side of the wing is a nice, round circle, for smooth movement. Once cut, paint the wings to match your costume – a coat of silver spray paint made our cardboard shine bright.”_

[Read more](https://hackspace.raspberrypi.org/issues/23) pages 78 to 81, [download PDF](https://magazines-static.raspberrypi.org/issues/full_pdfs/000/000/134/original/HackSpaceMagazine23.pdf?1568741893).

Adafruit Feather takes flight with the SparkFun Thing Plus Artemis
------------------------------------------------------------------

[![Adafruit Feather takes flight with the SparkFun Thing Plus](https://cdn-blog.adafruit.com/uploads/2019/09/92419artemis.jpg)](https://blog.adafruit.com/2019/09/19/adafruit-feather-takes-flight-with-the-sparkfun-thing-plus-artemis-sparkfun-adafruit/)

Adafruit Feather takes flight with the [SparkFun Thing Plus – Artemis](https://www.sparkfun.com/products/15574). AND: it appears CircuitPython support is _“a topic of discussion for sure”_! – [Twitter](https://twitter.com/sparkfun/status/1175099450072666113).

The latest SparkFun board is Feather-compatible! [This is the fifth](https://www.sparkfun.com/categories/tags/feather) SparkFun Adafruit Feather-compatible board (not including the Particle boards which are Feather format as well).

> _“To make the Thing Plus even easier to use, we’ve moved a few pins around to make the board Feather compatible…“_

[![Awesome Feather](https://cdn-blog.adafruit.com/uploads/2019/09/92419feathers.jpg)](https://github.com/adafruit/awesome-feather/)

Feather is a complete line of development boards that are both standalone and stackable. They’re able to be powered by LiPo batteries for on-the-go use or by their micro-USB plugs for stationary projects. Feathers are flexible, portable, and as light as their namesake. FeatherWings are stacking boards and add functionality and room for prototyping. At its core, Feather is a complete ecosystem of products – and the best way to get your project flying.

The Feathers at Adafruit are open source. Adafruit encourages other companies to utilize this form factor to maximize compatibility with dozens of pre-existing boards.

Check out awesome-feather for a complete list! – [github.com/adafruit/awesome-feather](https://github.com/adafruit/awesome-feather/).

Meet GIZMO!
-----------

[![Gizmo](https://cdn-blog.adafruit.com/uploads/2019/09/92419gizmo.jpg)](https://www.adafruit.com/product/4367)

Meet the new Circuit Playground TFT Gizmo, a Bolt-on Display + Audio Amplifier – [Adafruit](https://www.adafruit.com/product/4367).

Extend and expand your Circuit Playground projects with a bolt on TFT Gizmo that lets you add a lovely color display in a sturdy and reliable fashion. This PCB looks just like a round TFT breakout but has permanently affixed M3 standoffs that act as mechanical and electrical connections.

Once attached you’ll get a 1.54” 240×240 IPS display with backlight control, two 3-pin STEMMA connectors for attaching NeoPixel strips or servos, and a Class D audio amplifier with a Molex PicoBlade connector that can plug on one of our li’l speakers.

This is a great companion for our Circuit Playground Express or Bluefruit boards thanks to their fast SPI hardware speeds, and it works in CircuitPython. It comes with a PCB that has pre-soldered standoffs attached and 12x M3 screws for attachment.

CircuitPython and Mu book!
--------------------------

[![CircuitPython and Mu book](https://cdn-blog.adafruit.com/uploads/2019/09/92419bpbook01.jpg)](https://techbookfest.org/event/tbf07/circle/5645284751179776)

[![CircuitPython and Mu book](https://cdn-blog.adafruit.com/uploads/2019/09/92419bpbook02.jpg)](https://techbookfest.org/event/tbf07/circle/5645284751179776)

[![CircuitPython and Mu book](https://cdn-blog.adafruit.com/uploads/2019/09/92419bpbook03.jpg)](https://techbookfest.org/event/tbf07/circle/5645284751179776)

[![CircuitPython and Mu book](https://cdn-blog.adafruit.com/uploads/2019/09/92419booth.jpg)](https://techbookfest.org/event/tbf07/circle/5645284751179776)

Lots of activity and more for the CircuitPython & Mu book that is coming soon from Japan, including shirts! – [STEAM TOKYO](https://techbookfest.org/event/tbf07/circle/5645284751179776).

Introduction to CircuitPython class in Canton, CT
-------------------------------------------------

[![Introduction to CircuitPython class](https://cdn-blog.adafruit.com/uploads/2019/09/92419ctclass.jpg)](https://www.nextgensmartypants.com/product/circuit-python-shop/)

For individuals (Ages 10 – Adult) who love circuits or coding, check out this Introduction to CircuitPython class at NextGen SmartyPants in Canton, Connecticut USA – [nextgensmartypants.com](https://www.nextgensmartypants.com/product/circuit-python-shop/).

News from around the web!
-------------------------

[![badges](https://cdn-blog.adafruit.com/uploads/2019/09/92419badgeholder.jpg)](https://twitter.com/MacInspires/status/1174456811065356289)

A nice laser cut holder for all of the PyBadges at MacInspires – [Twitter](https://twitter.com/MacInspires/status/1174456811065356289).

[![Mike](https://cdn-blog.adafruit.com/uploads/2019/09/92419mike.jpg)](https://twitter.com/driscollis/status/1174333145736462337)

Mike, from Mouse vs Python, has his PyBadge up and running – [Twitter](https://twitter.com/driscollis/status/1174333145736462337).

[![Mask 13](https://cdn-blog.adafruit.com/uploads/2019/09/92419mask13.jpg)](https://youtu.be/8wqGA6usSbc)

Silver Mask with moving eyes with ADABOX 013 – YouTube via [Twitter](https://twitter.com/scottturneruon/status/1175806089331429377).

[![Spectral Foxes ](https://cdn-blog.adafruit.com/uploads/2019/09/92419fox.gif)](https://www.instagram.com/p/B2q9jH4HeEY/?igshid=1nylrsqrc50k4)

Presenting a pair of Spectral Foxes – [Instagram](https://www.instagram.com/p/B2q9jH4HeEY/?igshid=1nylrsqrc50k4).

[![Jeff board](https://cdn-blog.adafruit.com/uploads/2019/09/92419jeffboard.jpg)](https://twitter.com/jeffwurz/status/1175141831635423232)

More progress on Jeff’s CircuitPython board – [Twitter](https://twitter.com/jeffwurz/status/1175141831635423232).

[![CP badge life](https://cdn-blog.adafruit.com/uploads/2019/09/92419kevinbl.jpg)](https://twitter.com/kevinneubauer/status/1175122642598289409)

Kevin’s CircuitPython based custom conference badge is looking great! – [Twitter](https://twitter.com/kevinneubauer/status/1175122642598289409).

[![PyPortal IoT Plant Monitor](https://cdn-blog.adafruit.com/uploads/2019/09/92419pyportal_ms.jpg)](https://learn.adafruit.com/using-microsoft-azure-iot-with-circuitpython)

PyPortal IoT Plant Monitor with Microsoft Azure IoT and CircuitPython. Monitor your plant’s vitals by combining CircuitPython with Microsoft Azure IoT – [learn.adafruit.com](https://learn.adafruit.com/using-microsoft-azure-iot-with-circuitpython)

[![Eyes](https://cdn-blog.adafruit.com/uploads/2019/09/92419dragoneyes.gif)](https://twitter.com/KegawaCreation/status/1174776692952444929)

Anrhok work in progress, eyes made by Lucky and Hige – [Twitter](https://twitter.com/KegawaCreation/status/1174776692952444929).

What can you fit into an 8×8 pixel display? Find out: [Christian](https://twitter.com/isziaui/status/1175706349998661633) is bringing some PewPews to the Creative Coding ZH meetup and will show how to program simple games or demos in CircuitPython – [Meetup](https://www.meetup.com/creative-coding/events/264988094/).

[![Daniel](https://cdn-blog.adafruit.com/uploads/2019/09/92419danielpb.jpg)](https://twitter.com/chendaniely/status/1174058510285512705)

Daniel’s excellent PyBadge – [Twitter](https://twitter.com/chendaniely/status/1174058510285512705).

Building Custom Deep Learning Based OCR models by Anuj Sable – [nanonets.com](https://nanonets.com/blog/attention-ocr-for-text-recogntion/)

[![Lamp](https://cdn-blog.adafruit.com/uploads/2019/09/92419lamp.gif)](https://manoj.ninja/articles/2019/09/19/2019-building-a-gesture-controlled-lamp)

Building a micro:bit gesture controlled lamp – [manjo.ninja](https://manoj.ninja/articles/2019/09/19/2019-building-a-gesture-controlled-lamp).

[![Learn Python](https://cdn-blog.adafruit.com/uploads/2019/09/92419introtopython.jpg)](https://www.youtube.com/playlist?list=PLlrxD0HtieHhS8VzuMCfQD4uJ9yne1mE6)

Microsoft has a 44 part series on [YouTube, all about Python](https://www.youtube.com/playlist?list=PLlrxD0HtieHhS8VzuMCfQD4uJ9yne1mE6) –

> _“Probably the largest hurdle when learning any new programming language is simply knowing where to get started. This is why we, Chris and Susan, decided to create this series about Python for Beginners! Even though we won’t cover everything there is to know about Python in the course, we want to make sure we give you the foundation on programming in Python, starting from common everyday code and scenarios. At the end of the course, you’ll be able to go and learn on your own, for example with docs, tutorials, or books.”_

[![Amp Hour](https://cdn-blog.adafruit.com/uploads/2019/09/92419amphour.jpg)](https://theamphour.com/458-an-interview-with-ken-burns/)

[The latest Amp Hour electronics podcast](https://theamphour.com/458-an-interview-with-ken-burns/) had Ken Burns of TinyCircuits – towards the end of the interview there are some CircuitPython mentions around the 1 hour 22 min mark.

[![Laser Crown](https://cdn-blog.adafruit.com/uploads/2019/09/92419laser_crown.png)](https://www.instructables.com/id/Laser-Crown/)

Laser crown! – [Instructables](https://www.instructables.com/id/Laser-Crown/).

[![Comodore 64](https://cdn-blog.adafruit.com/uploads/2019/09/92419comodore.jpg)](https://www.adafruit.com)

Jepler was working on a cool Commodore 64 + CircuitPython project!

[![Robo HAT](https://cdn-blog.adafruit.com/uploads/2019/09/92419robo-hat-update-4_jpg_project-body.jpg)](https://www.crowdsupply.com/robotics-masters/robo-hat-mm1/updates/testing-jig-arrived)

Robo HAT MM1 by Robotics Masters – their testing jig arrived – [Crowdy Supply](https://www.crowdsupply.com/robotics-masters/robo-hat-mm1/updates/testing-jig-arrived).

KiPro is Professional support for KiCad. Offers private bug reports, customized hardware and feature release schedules [kipro-pcb.com](https://www.kipro-pcb.com/).

[![100k pi](https://cdn-blog.adafruit.com/uploads/2019/09/92419moon.png)](https://moon.hoyd.net/matematikk/2913)

Visualizing 100k decimals of Pi, Tau and e with Python – [moon.hoyd.net](https://moon.hoyd.net/matematikk/2913).

Token scanning – [GitHub](https://developer.github.com/partnerships/token-scanning/).

Lectures in Quantitative Economics with Python – [PDF](https://lectures.quantecon.org/_downloads/pdf/py/Quantitative%20Economics%20with%20Python.pdf).

A Python alternative to Docker – [Matt Layman](https://www.mattlayman.com/blog/2019/python-alternative-docker/).

[![Colab](https://cdn-blog.adafruit.com/uploads/2019/09/92419colab.jpg)](https://learn.adafruit.com/basic-tensorflow-object-recognition-in-the-cloud-google-colab?view=all)

Basic TensorFlow Object Recognition on any Computer or iOS device with Google Colab – [Adafruit](https://learn.adafruit.com/basic-tensorflow-object-recognition-in-the-cloud-google-colab?view=all).

[An absolute beginners guide to nRF52840](https://medium.com/@teja.chintalapati/an-abosulte-beginners-guide-to-nrf52840-b579cfe1fc1c) by Teja Chintalapati.

[Brian Ringley](https://twitter.com/brianringley/status/1170351203861094400) list of construction robotics – [Google Doc](https://docs.google.com/spreadsheets/d/1tJFsyj3bAW_d-02T8BZXBXuVK-2kOjPQvh5STzWgymo/edit#gid=0).

[![Python bundle](https://cdn-blog.adafruit.com/uploads/2019/09/92419pythonbundle.jpg)](https://www.humblebundle.com/level-up-your-python)

A few days left for the Humble Level Up Your Python Bundle, pay what you want and help charity – [humblebundle.com/level-up-your-python](https://www.humblebundle.com/level-up-your-python).

[![PyGame](https://cdn-blog.adafruit.com/uploads/2019/09/92419pygamerp.png)](https://realpython.com/pygame-a-primer/)

PyGame: A Primer on Game Programming in Python by Jon Fincher – [Real Python](https://realpython.com/pygame-a-primer/).

14,000 word Technical Deep Dive about RS-232, WiFi modems and networking in C64 OS, with some intro talk about Chess and turn-based network games – [C64OS](http://www.c64os.com/post/chess_c64os_networking) via [Twitter](https://twitter.com/gregnacu/status/1175094880894365697).

Inside Tesla’s Neural Processor In The FSD Chip – [wikichip.org](https://fuse.wikichip.org/news/2707/inside-teslas-neural-processor-in-the-fsd-chip/)

100,000 AI-Generated Faces – Free to use! – [generated.photos](https://generated.photos/) & [Google drive photos](https://drive.google.com/drive/folders/1wSy4TVjSvtXeRQ6Zr8W98YbSuZXrZrgY).

[Artbreeder](https://artbreeder.com/) – Create beautiful, wild and weird images.

ImageNet Roulette is a provocation designed to help us see into the ways that humans are classified in machine learning systems. It uses a neural network trained on the “Person” categories from the ImageNet dataset which has over 2,500 labels used to classify images of people – [imagenet-roulette.paglen.com](https://imagenet-roulette.paglen.com/)

Halloween custom prints – [Print all over me](https://paom.com/search?type=product&q=*halloween*+tag:public).

Balancing Makers and Takers to scale and sustain Open Source – [DRIES BUYTAERT](https://dri.es/balancing-makers-and-takers-to-scale-and-sustain-open-source).

Software Engineering at Google – [PDF](https://arxiv.org/pdf/1702.01715.pdf).

[![Moore's Law](https://cdn-blog.adafruit.com/uploads/2019/09/92419law.jpg)](https://twitter.com/page_eco/status/1168832625269563393)

Moore’s law visualization, predictions vs actual growth in transistor count – [Twitter](https://twitter.com/SalimChemlal/status/1169443543842095104).

[![Serpente](https://cdn-blog.adafruit.com/uploads/2019/09/92419serp.jpg)](https://www.adafruitdaily.com/2019/09/17/python-snakes-its-way-to-the-stm32-serpente-and-more/)

[![Easy](https://cdn-blog.adafruit.com/uploads/2019/09/92719easyuf2.jpg)](https://twitter.com/arturo182/status/1174075172242022401)

And on that note, this is great to hear – [Twitter](https://twitter.com/arturo182/status/1174075172242022401).

> _“Thanks to Adafruit’s UF2 bootloader, the update process is super easy.”_

Bugfix and DMCA Lawsuit Progress NeTV2 – [Crowd Supply](https://www.crowdsupply.com/alphamax/netv2/updates/bugfix-and-dmca-lawsuit-progress).

How did we miss this? Mouser acquired Crowd Supply LAST YEAR – [Crowd Supply](https://blog.crowdsupply.com/2018/10/03/crowd-supply-has-been-acquired/).

#ICYDNCI What was the most popular, most clicked link, in [last week’s newsletter](https://www.adafruitdaily.com/2019/09/17/python-snakes-its-way-to-the-stm32-serpente-and-more/)? [Serpente – A Tiny CircuitPython Prototyping Board](https://www.tindie.com/products/arturo182/serpente-a-tiny-circuitpython-prototyping-board/).

PyDev of the Week: Peter Farrell – [Mouse vs Python](https://www.blog.pythonlibrary.org/2019/09/23/pydev-of-the-week-peter-farrell/).

CircuitPython Weekly Meeting for September 23rd, 2019 [on YouTube](https://youtu.be/DWySqjttJng) and [on diode.zone](https://diode.zone/videos/watch/8fe5fe02-f1a7-4d51-a268-01d814612736).

Coming soon
-----------

[![BeagleBone AI](https://cdn-blog.adafruit.com/uploads/2019/09/92419boneai.jpg)](https://beagleboard.org/ai)

The new [BeagleBone AI](https://beagleboard.org/ai) was released! We have one – we’re going to get [BLINKA going on it first](https://circuitpython.org/blinka)!

[![Updates coming soon to Bluefruit](https://cdn-blog.adafruit.com/uploads/2019/09/92419bluefruitupt.jpg)](https://youtu.be/XsFt8I0q0R0)

Updates coming soon to Bluefruit! – [YouTube](https://youtu.be/XsFt8I0q0R0).

[![STEMMA Relay Breakout](https://cdn-blog.adafruit.com/uploads/2019/09/92419stemma.png)](https://www.adafruit.com/new)

STEMMA Relay Breakout. This all-SMT breakout lets you control a 60W relay with a plug-n-play 3-pin JST PH cable connection. Clicky clacky!

[![PyBadge cases](https://cdn-blog.adafruit.com/uploads/2019/09/92419pybadgec01.jpg)](https://www.adafruit.com/?q=pybadge)

[![PyBadge cases](https://cdn-blog.adafruit.com/uploads/2019/09/92419pybadgec02.jpg)](https://www.adafruit.com/?q=pybadge)

[![PyBadge cases](https://cdn-blog.adafruit.com/uploads/2019/09/92419pybadgec03.jpg)](https://www.adafruit.com/?q=pybadge)

Working on some new cases for the [PyBadge](https://www.adafruit.com/?q=pybadge)!

[![WiFi backpack](https://cdn-blog.adafruit.com/uploads/2019/09/92419sam01.jpg)](https://twitter.com/bwshockley/status/1175510380732387328?s=11)

[![WiFi backpack](https://cdn-blog.adafruit.com/uploads/2019/09/92419sam02.jpg)](https://twitter.com/bwshockley/status/1175510380732387328?s=11)

Mini SAM + WiFi backpack, maybe? – [Twitter](https://twitter.com/bwshockley/status/1175510380732387328?s=11).

**Introducing Glider**

[![Glider](https://cdn-blog.adafruit.com/uploads/2019/09/92419scottglide.jpg)](https://github.com/adafruit/glider)

Glider is a portable mobile app aimed at making wireless editing of Python code really easy and fun. We’ll have more soon, this is the start! – [GitHub](https://github.com/adafruit/glider) & [Twitter](https://twitter.com/tannewt/status/1175436660902772736).

New Learn Guides!
-----------------

[![CircUp](https://cdn-blog.adafruit.com/uploads/2019/09/92419circup.jpg)](https://learn.adafruit.com/keep-your-circuitpython-libraries-on-devices-up-to-date-with-circup)

[Keep your CircuitPython libraries on devices easily updated with CircUp](https://learn.adafruit.com/keep-your-circuitpython-libraries-on-devices-up-to-date-with-circup) from [Melissa LeBlanc-Williams](https://learn.adafruit.com/users/MakerMelissa)

[![Bluefruit](https://cdn-blog.adafruit.com/uploads/2019/09/92419bfguide.jpg)](https://learn.adafruit.com/adafruit-circuit-playground-bluefruit)

[Adafruit Circuit Playground Bluefruit](https://learn.adafruit.com/adafruit-circuit-playground-bluefruit) from [Kattni](https://learn.adafruit.com/users/kattni)

[Adafruit Hallowing M4](https://learn.adafruit.com/adafruit-hallowing-m4) from [Kattni](https://learn.adafruit.com/users/kattni)

Team updates!
-------------

**Bryan**

[![Bryan](https://cdn-blog.adafruit.com/uploads/2019/09/92419bryan01.jpg)](https://circuitpython.org/)

![Bryan](https://cdn-blog.adafruit.com/uploads/2019/09/92419mpu.png)

> _“This week I finished up and released the SSD1305 framebuf driver to be used with the upcoming Large OLED Bonnet. If I may say so myself, it looks great! I also assembled and started working on the driver for the upcoming MPU-6050 STEMMA QT compatible 6-axis Accelerometer and Gyroscope.”_

**Jepler**

[![Jepler](https://cdn-blog.adafruit.com/uploads/2019/09/92419jepler.jpg)](https://circuitpython.org/)

> _“This week, my main work was more research about DAC issues on the boards with samd51 microcontrollers, like the Metro M4 Express. A pull request improved various problems when the DACs were used for simple analog out or audio out, but some strange behavior remains where high amplitude square waves are concerned. I personally suspect there might be gremlins in the silicon at this point. Along the way, I learned how to use my scope’s pass/fail mode to record how often an anomaly occurred when looping a short sample via CircuitPython’s AudioOut. Answer: Less than 0.5% of the time in this test, after employing a workaround.”_

**Kattni**

> _“The Circuit Playground Bluefruit guide has been published! I found a number of bugs during testing, and we’ve since fixed them all. This week, I’m working on the Hallowing M4 guide. If you’re looking for how to get going with your Hallowing M4, keep an eye out for that to be published soon! After that, I’ll be adding three Bluetooth examples to the Circuit Playground Bluefruit guide. They’ll provide a starting point for using CircuitPython with the Bluetooth features of your CPB!”_

**Lucian**

> _“We just wrapped up AnalogIO for the STM32 today after getting held up by some tricky bugs. Now that that’s completed, I’ll be moving on to expanding the implementation of I2C and the rest of BusIO using a new implementation of peripherals specific to the STM32. This will enable a bunch of new modules and breakout boards to be used with CircuitPython! I’ll also be working on support for new F4 dev boards.”_

**Melissa**

> _“Just finished up writing a learn guide for a new utility called CircUp that allows easy maintenance of CircuitPython libraries across your devices. You can check out the learn guide [here](https://learn.adafruit.com/keep-your-circuitpython-libraries-on-devices-up-to-date-with-circup). I’ve gone through the displayio examples making some minor updates and updated the corresponding CircuitPython displayio learn guide pages. I’ve also been adding several new boards to the circuitpython.org website under the Downloads page. I took the Arduino ST7735 Library and split up the graphicstest example into 4 different examples so it would be easier to follow along with newer boards such as the HalloWing M4. I also fixed a bug in the CircuitPython Seesaw library that wasn’t allowing the NeoTrellis and MiniTFT boards to work correctly on the latest versions of CircuitPython. Now I’m working on going through updating the monochrome OLED learn guide pages to reflect some of the recently added displayio drivers.”_

Updated Guides – Now With More Python!
--------------------------------------

**You can use CircuitPython libraries on Raspberry Pi!** We’re updating all of our CircuitPython guides to show how to wire up sensors to your Raspberry Pi, and load the necessary CircuitPython libraries to get going using them with Python. We’ll be including the updates here so you can easily keep track of which sensors are ready to go. Check it out!

Keep checking back for more updated guides!

CircuitPython Libraries!
------------------------

[![CircuitPython Libraries](https://cdn-blog.adafruit.com/uploads/2019/09/92419blinka.png)](https://circuitpython.org/libraries)

CircuitPython support for hardware continues to grow. We are adding support for new sensors and breakouts all the time, as well as improving on the drivers we already have. As we add more libraries and update current ones, you can keep up with all the changes right here!

For the latest drivers, download the [Adafruit CircuitPython Library Bundle](https://circuitpython.org/libraries).

If you’d like to contribute, CircuitPython libraries are a great place to start. Have an idea for a new driver? File an issue on [CircuitPython](https://github.com/adafruit/circuitpython/issues)! Interested in helping with current libraries? Check out [this GitHub issue on CircuitPython](https://github.com/adafruit/circuitpython/issues/1246) for an overview of the State of the CircuitPython Libraries, updated each week. We’ve included open issues from the library issue lists, and details about repo-level issues that need to be addressed. We have a guide on [contributing to CircuitPython with Git and Github](https://learn.adafruit.com/contribute-to-circuitpython-with-git-and-github) if you need help getting started. You can also find us in the #circuitpython channel on the [Adafruit Discord](https://adafru.it/discord). Feel free to contact Kattni (@kattni) with any questions.

You can check out this [list of all the CircuitPython libraries and drivers available](https://github.com/adafruit/Adafruit_CircuitPython_Bundle/blob/master/circuitpython_library_list.md).

The current number of CircuitPython libraries is **187**!

**New Libraries!**

Here’s this week’s new CircuitPython libraries:

*   [Adafruit\_CircuitPython\_SSD1305](https://github.com/adafruit/Adafruit_CircuitPython_SSD1305)
*   [Adafruit\_CircuitPython\_ATECC](https://github.com/adafruit/Adafruit_CircuitPython_ATECC)

**Updated Libraries!**

Here’s this week’s updated CircuitPython libraries:

*   [Adafruit\_CircuitPython\_TLC59711](https://github.com/adafruit/Adafruit_CircuitPython_TLC59711)
*   [Adafruit\_CircuitPython\_DS2413](https://github.com/adafruit/Adafruit_CircuitPython_DS2413)
*   [Adafruit\_CircuitPython\_HTU21D](https://github.com/adafruit/Adafruit_CircuitPython_HTU21D)
*   [Adafruit\_CircuitPython\_FancyLED](https://github.com/adafruit/Adafruit_CircuitPython_FancyLED)
*   [Adafruit\_CircuitPython\_miniesptool](https://github.com/adafruit/Adafruit_CircuitPython_miniesptool)
*   [Adafruit\_CircuitPython\_MCP3xxx](https://github.com/adafruit/Adafruit_CircuitPython_MCP3xxx)
*   [Adafruit\_CircuitPython\_IRRemote](https://github.com/adafruit/Adafruit_CircuitPython_IRRemote)
*   [Adafruit\_CircuitPython\_MPRLS](https://github.com/adafruit/Adafruit_CircuitPython_MPRLS)
*   [Adafruit\_CircuitPython\_BME280](https://github.com/adafruit/Adafruit_CircuitPython_BME280)
*   [Adafruit\_CircuitPython\_RTTTL](https://github.com/adafruit/Adafruit_CircuitPython_RTTTL)
*   [Adafruit\_CircuitPython\_DS18X20](https://github.com/adafruit/Adafruit_CircuitPython_DS18X20)
*   [Adafruit\_CircuitPython\_SHT31D](https://github.com/adafruit/Adafruit_CircuitPython_SHT31D)
*   [Adafruit\_CircuitPython\_MotorKit](https://github.com/adafruit/Adafruit_CircuitPython_MotorKit)
*   [Adafruit\_CircuitPython\_SD](https://github.com/adafruit/Adafruit_CircuitPython_SD)
*   [Adafruit\_CircuitPython\_Thermal\_Printer](https://github.com/adafruit/Adafruit_CircuitPython_Thermal_Printer)
*   [Adafruit\_CircuitPython\_AVRprog](https://github.com/adafruit/Adafruit_CircuitPython_AVRprog)
*   [Adafruit\_CircuitPython\_ImageLoad](https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad)
*   [Adafruit\_CircuitPython\_MSA301](https://github.com/adafruit/Adafruit_CircuitPython_MSA301)
*   [Adafruit\_CircuitPython\_Nunchuk](https://github.com/adafruit/Adafruit_CircuitPython_Nunchuk)
*   [Adafruit\_CircuitPython\_MPR121](https://github.com/adafruit/Adafruit_CircuitPython_MPR121)
*   [Adafruit\_CircuitPython\_ADXL34x](https://github.com/adafruit/Adafruit_CircuitPython_ADXL34x)
*   [Adafruit\_CircuitPython\_PCT2075](https://github.com/adafruit/Adafruit_CircuitPython_PCT2075)
*   [Adafruit\_CircuitPython\_Requests](https://github.com/adafruit/Adafruit_CircuitPython_Requests)
*   [Adafruit\_CircuitPython\_ESP32SPI](https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI)
*   [Adafruit\_CircuitPython\_CircuitPlayground](https://github.com/adafruit/Adafruit_CircuitPython_CircuitPlayground)
*   [Adafruit\_CircuitPython\_SSD1306](https://github.com/adafruit/Adafruit_CircuitPython_SSD1306)
*   [Adafruit\_CircuitPython\_HX8357](https://github.com/adafruit/Adafruit_CircuitPython_HX8357)
*   [Adafruit\_CircuitPython\_ST7789](https://github.com/adafruit/Adafruit_CircuitPython_ST7789)
*   [Adafruit\_CircuitPython\_ST7735](https://github.com/adafruit/Adafruit_CircuitPython_ST7735)
*   [Adafruit\_CircuitPython\_ST7735R](https://github.com/adafruit/Adafruit_CircuitPython_ST7735R)
*   [Adafruit\_CircuitPython\_SSD1331](https://github.com/adafruit/Adafruit_CircuitPython_SSD1331)
*   [Adafruit\_CircuitPython\_ILI9341](https://github.com/adafruit/Adafruit_CircuitPython_ILI9341)
*   [Adafruit\_CircuitPython\_SSD1351](https://github.com/adafruit/Adafruit_CircuitPython_SSD1351)
*   [Adafruit\_CircuitPython\_seesaw](https://github.com/adafruit/Adafruit_CircuitPython_seesaw)
*   [Adafruit\_CircuitPython\_FeatherWing](https://github.com/adafruit/Adafruit_CircuitPython_FeatherWing)
*   [Adafruit\_CircuitPython\_MAX31855](https://github.com/adafruit/Adafruit_CircuitPython_MAX31855)
*   [Adafruit\_CircuitPython\_SimpleIO](https://github.com/adafruit/Adafruit_CircuitPython_SimpleIO)
*   [Adafruit\_CircuitPython\_GPS](https://github.com/adafruit/Adafruit_CircuitPython_GPS)

**PyPI Download Stats!**

We’ve written a special library called Adafruit Blinka that makes it possible to use CircuitPython Libraries on [Raspberry Pi and other compatible single-board computers](https://learn.adafruit.com/circuitpython-on-raspberrypi-linux/). Adafruit Blinka and all the CircuitPython libraries have been deployed to PyPI for super simple installation on Linux! Here are the top 10 CircuitPython libraries downloaded from PyPI in the last week, including the total downloads for those libraries:

Library

Last Week

Total

Adafruit-Blinka

1472

46065

Adafruit\_CircuitPython\_BusDevice

822

21636

Adafruit\_CircuitPython\_MCP230xx

342

6761

Adafruit\_CircuitPython\_Register

171

7074

Adafruit\_CircuitPython\_Thermal\_Printer

164

1067

Adafruit\_CircuitPython\_ESP32SPI

143

1870

Adafruit\_CircuitPython\_NeoPixel

128

6296

Adafruit\_CircuitPython\_Motor

128

5228

Adafruit\_CircuitPython\_PCA9685

123

4869

Adafruit\_CircuitPython\_MotorKit

118

2603

Upcoming events!
----------------

[![Open source hardware month](https://cdn-blog.adafruit.com/uploads/2019/09/92419oshwmonth.jpg)](https://www.oshwa.org/2019/07/26/october-is-open-hardware-month-2/)

[October is Open Hardware Month @ Open Source Hardware Association](https://www.oshwa.org/2019/07/26/october-is-open-hardware-month-2/).

> _“October is Open Hardware Month! Check out the [Open Hardware Month website](http://ohm.oshwa.org/). Host an event, find a local event, or [certify](https://certification.oshwa.org/) your hardware to support Open Source Hardware. We are providing resources and asking you, the community, to host small, local events in the name of open source hardware. Tell us about your October event by [filling out the form](https://docs.google.com/forms/d/e/1FAIpQLSfjvJmcRXbpgjRACgY_BbaDzQZRa6wxEcP-xwaBpC0X6mvsPw/viewform). Your event will be featured on [OSHWA’s Open Hardware Month page](http://ohm.oshwa.org/) (provided you have followed OSHWA’s rules listed on the [“Do’s and Don’ts”](http://ohm.oshwa.org/dos-and-donts/) page).”_

[Read more](https://www.oshwa.org/2019/07/26/october-is-open-hardware-month-2/), [Tweet for speakers in 2020](https://twitter.com/ohsummit/status/1154881782677831680), and Open Hardware Month @ [http://ohm.oshwa.org/](http://ohm.oshwa.org/)

[![Ada Lovelace Day](https://cdn-blog.adafruit.com/uploads/2019/09/92419ald.jpg)](https://findingada.com/)

Ada Lovelace Day (ALD) is an international celebration of the achievements of women in science, technology, engineering and maths (STEM). It aims to increase the profile of women in STEM and, in doing so, create new role models who will encourage more girls into STEM careers and support women already working in STEM – [findingada.com](https://findingada.com/).

[![PyCon DE](https://cdn-blog.adafruit.com/uploads/2019/09/92419pyconde.jpg)](https://de.pycon.org/)

PyCon DE & PyData Berlin, Germany // October 9 – 13 2019. Main conference, 3 days of talks and workshops. More than 100 sessions dedicated to PyData (artificial intelligence, machine learning, ethics…) and Python topics (programming, DevOps, Web, Django…) – [de.pycon.org](https://de.pycon.org/).

[![micro:bit Live 2019](https://cdn-blog.adafruit.com/uploads/2019/09/92419mblive.png)](https://microbit.org/en/2019-04-12-microbit-live/)

micro:bit Live 2019 is coming to BBC MediaCityUK, Greater Manchester, England on October 4-5. This will be the very first annual gathering of the global micro:bit community of educators and partners – [micro:bit](https://microbit.org/en/2019-04-12-microbit-live/).

[![Hackaday Superconference](https://cdn-blog.adafruit.com/uploads/2019/09/92419supercon.jpg)](https://hackaday.io/superconference/)

Hackaday Superconference is November 15th, 16th, and 17th in Pasadena, California, USA. The Hackaday Superconference is returning for another 3 full days of technical talks, badge hacking, and hands-on workshops: [Eventbrite](https://www.eventbrite.com/e/hackaday-superconference-2019-tickets-60129236164?aff=0626com) & [hackaday.io](https://hackaday.io/superconference/)

Latest releases
---------------

CircuitPython’s stable release is [4.1.0](https://github.com/adafruit/circuitpython/releases/latest) and its unstable release is [5.0.0-alpha.4](https://github.com/adafruit/circuitpython/releases). New to CircuitPython? Start with our [Welcome to CircuitPython Guide](https://learn.adafruit.com/welcome-to-circuitpython).

[20190922](https://github.com/adafruit/Adafruit_CircuitPython_Bundle/releases/latest) is the latest CircuitPython library bundle.

[v1.11](https://micropython.org/download) is the latest MicroPython release. Documentation for it is [here](http://docs.micropython.org/en/latest/pyboard/).

[3.7.4](https://www.python.org/downloads/) is the latest Python release. The latest pre-release version is [3.8.0b4](https://www.python.org/download/pre-releases/).

[1399 Stars](https://github.com/adafruit/circuitpython/stargazers) Like CircuitPython? [Star it on GitHub!](https://github.com/adafruit/circuitpython)

Call for help – CircuitPython messaging to other languages!
-----------------------------------------------------------

[![Hello world](https://cdn-blog.adafruit.com/uploads/2019/09/92419helloworld.jpg)](https://github.com/adafruit/circuitpython/issues/1098)

We [posted on the Adafruit blog](https://blog.adafruit.com/2018/08/15/help-bring-circuitpython-messaging-to-other-languages-circuitpython/) about bringing CircuitPython messaging to other languages, one of the exciting features of CircuitPython 4.x is translated control and error messages. Native language messages will help non-native English speakers understand what is happening in CircuitPython even though the Python keywords and APIs will still be in English. If you would like to help, [please post](https://github.com/adafruit/circuitpython/issues/1098) to the main issue on GitHub and join us on [Discord](https://adafru.it/discord).

We made this graphic with translated text, we could use your help with that to make sure we got the text right, please check out the text in the image – if there is anything we did not get correct, please let us know. Dan sent me this [handy site too](http://helloworldcollection.de/#Human).

jobs.adafruit.com – Find a dream job, find great candidates!
------------------------------------------------------------

[![jobs.adafruit.com](https://cdn-blog.adafruit.com/uploads/2019/09/92419jobs.jpg)](https://jobs.adafruit.com/)

[jobs.adafruit.com](https://jobs.adafruit.com/) has returned and folks are posting their skills (including CircuitPython) and companies are looking for talented makers to join their companies – from Digi-Key, to Hackaday, Microcenter, Raspberry Pi and more.

14,151 thanks!
--------------

[![14,151](https://cdn-blog.adafruit.com/uploads/2019/09/9241914kdiscord.jpg)](https://adafru.it/discord)

[![Adafruit Discord](https://discordapp.com/api/guilds/327254708534116352/embed.png?style=banner3)](https://discord.gg/adafruit)

The Adafruit Discord community, where we do all our CircuitPython development in the open, reached over 14,151 humans, thank you! Join today! [https://adafru.it/discord](https://adafru.it/discord)

[![Chart](https://cdn-blog.adafruit.com/uploads/2019/09/92419discordchart.jpg)](https://adafru.it/discord)

We just reached 14,000 humans, here’s what that looks like over time!

Discord now offers “server boosts”. We have 13 on our server (level 2) and if we get to 50 boosts we get to level 3 and some other good features for the community: +100 emojis for a total of 250, 384 Kbps audio, vanity URL, 100 mb uploads for all members (and all the things we have now, like the server banner). Stop by and boost! [https://adafru.it/discord](https://adafru.it/discord).

ICYMI – In case you missed it
-----------------------------

[![ICYMI](https://cdn-blog.adafruit.com/uploads/2019/09/92419icymi.jpg)](https://www.youtube.com/playlist?list=PLjF7R1fz_OOXRMjM7Sm0J2Xt6H81TdDev)

The wonderful world of Python on hardware! This is our first video-newsletter-podcast that we’ve started! The news comes from the Python community, Discord, Adafruit communities and more. It’s part of the weekly newsletter, then we have a segment on ASK an ENGINEER and this is the video slice from that! The complete Python on Hardware weekly videocast [playlist is here](https://www.youtube.com/playlist?list=PLjF7R1fz_OOXRMjM7Sm0J2Xt6H81TdDev).

This video podcast is on [iTunes](https://itunes.apple.com/us/podcast/python-on-hardware/id1451685192?mt=2), [YouTube](https://www.youtube.com/playlist?list=PLjF7R1fz_OOXRMjM7Sm0J2Xt6H81TdDev), [IGTV (Instagram TV](https://www.instagram.com/adafruit/channel/)), and [XML](https://itunes.apple.com/us/podcast/python-on-hardware/id1451685192?mt=2).

[Weekly community chat on Adafruit Discord server CircuitPython channel – Audio / Podcast edition](https://itunes.apple.com/us/podcast/circuitpython-weekly-meeting/id1451685016) – Audio from the Discord chat space for CircuitPython, meetings are usually Mondays at 2pm ET, this is the audio version on [iTunes](https://itunes.apple.com/us/podcast/circuitpython-weekly-meeting/id1451685016), Pocket Casts, [Spotify](https://adafru.it/spotify), and [XML feed](https://adafruit-podcasts.s3.amazonaws.com/circuitpython_weekly_meeting/audio-podcast.xml).

And lastly, we are working up a one-spot destination for all things podcast-able here – [podcasts.adafruit.com](https://podcasts.adafruit.com/)

Codecademy “Learn Hardware Programming with CircuitPython”
----------------------------------------------------------

[![Codecademy CircuitPython](https://cdn-blog.adafruit.com/uploads/2019/09/92419codecademy_python.png)](https://www.codecademy.com/learn/learn-circuitpython?utm_source=adafruit&utm_medium=partners&utm_campaign=circuitplayground&utm_content=pythononhardwarenewsletter)

Codecademy, an online interactive learning platform used by more than 45 million people, has teamed up with the leading manufacturer in STEAM electronics, Adafruit Industries, to create a coding course, “Learn Hardware Programming with CircuitPython”. The course is now available in the [Codecademy catalog](https://www.codecademy.com/learn/learn-circuitpython?utm_source=adafruit&utm_medium=partners&utm_campaign=circuitplayground&utm_content=pythononhardwarenewsletter).

Python is a highly versatile, easy to learn programming language that a wide range of people, from visual effects artists in Hollywood to mission control at NASA, use to quickly solve problems. But you don’t need to be a rocket scientist to accomplish amazing things with it. This new course introduces programmers to Python by way of a microcontroller — CircuitPython — which is a Python-based programming language optimized for use on hardware.

CircuitPython’s hardware-ready design makes it easier than ever to program a variety of single-board computers, and this course gets you from no experience to working prototype faster than ever before. Codecademy’s interactive learning environment, combined with Adafruit’s highly rated Circuit Playground Express, present aspiring hardware hackers with a never-before-seen opportunity to learn hardware programming seamlessly online.

Whether for those who are new to programming, or for those who want to expand their skill set to include physical computing, this course will have students getting familiar with Python and creating incredible projects along the way. By the end, students will have built their own bike lights, drum machine, and even a moisture detector that can tell when it’s time to water a plant.

Visit Codecademy to access the [Learn Hardware Programming with CircuitPython](https://www.codecademy.com/learn/learn-circuitpython?utm_source=adafruit&utm_medium=partners&utm_campaign=circuitplayground&utm_content=pythononhardwarenewsletter) course and Adafruit to purchase a [Circuit Playground Express](https://www.adafruit.com/product/3333).

Codecademy has helped more than 45 million people around the world upgrade their careers with technology skills. The company’s online interactive learning platform is widely recognized for providing an accessible, flexible, and engaging experience for beginners and experienced programmers alike. Codecademy has raised a total of $43 million from investors including Union Square Ventures, Kleiner Perkins, Index Ventures, Thrive Capital, Naspers, Yuri Milner and Richard Branson, most recently raising its $30 million Series C in July 2016.

Contribute!
-----------

The CircuitPython Weekly Newsletter is a CircuitPython community-run newsletter emailed every Tuesday. The complete [archives are here](https://www.adafruitdaily.com/category/circuitpython/). It highlights the latest CircuitPython related news from around the web including Python and MicroPython developments. To contribute, edit next week’s draft [on GitHub](https://github.com/adafruit/circuitpython-weekly-newsletter/tree/gh-pages/_drafts) and [submit a pull request](https://help.github.com/articles/editing-files-in-your-repository/) with the changes. Join our [Discord](https://adafru.it/discord) or [post to the forum](https://forums.adafruit.com/viewforum.php?f=60) for any further questions.