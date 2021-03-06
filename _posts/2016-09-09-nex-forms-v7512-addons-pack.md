---
title: 'NEX-Forms v7.5.12 + Addons Pack'
date: 2020-02-17T01:24:00+01:00
draft: false
---

**Kang Asu**

[![](https://1.bp.blogspot.com/-W0AHKaLFegw/Xjoq9_9lhjI/AAAAAAAARnM/Kmi9daKc5GAASo8mB2I4MnQ5TorcKdI_gCNcBGAsYHQ/s640/Re2Pcap_3_re2pcap.png)](https://1.bp.blogspot.com/-W0AHKaLFegw/Xjoq9_9lhjI/AAAAAAAARnM/Kmi9daKc5GAASo8mB2I4MnQ5TorcKdI_gCNcBGAsYHQ/s1600/Re2Pcap_3_re2pcap.png)

**Re2Pcap - Create PCAP file from raw HTTP request or response in seconds**

  
Re2Pcap is abbreviation for Request2Pcap and Response2Pcap. Community users can quickly create PCAP file using Re2Pcap and test them against [Snort](https://snort.org/ "Snort") rules.  
Re2Pcap allow you to quickly create PCAP file for raw HTTP request shown below

```
POST /admin/tools/iplogging.cgi HTTP/1.1  
Host: 192.168.13.31:80  
User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:60.0) Gecko/20100101 Firefox/60.0  
Accept: text/plain, */*; q=0.01  
Accept-Language: en-US,en;q=0.5  
Accept-Encoding: gzip, deflate  
Referer: [http://192.168.13.31:80/admin/tools/iplogging.html](http://192.168.13.31/admin/tools/iplogging.html)  
Content-Type: application/x-www-form-urlencoded; charset=UTF-8  
X-Requested-With: XMLHttpRequest  
Content-Length: 63  
Cookie: token=1e9c07e135a15e40b3290c320245ca9a  
Connection: close  
  
tcpdumpParams=tcpdump -z reboot -G 2 -i eth0&stateRequest=start
```

  

[](https://www.blogger.com/u/7/null)  
**Usage**

```
git clone [https://github.com/Cisco-Talos/Re2Pcap.git](https://github.com/Cisco-Talos/Re2Pcap.git)  
cd Re2Pcap/  
docker build -t re2pcap .  
docker run --rm --cap-add NET_ADMIN -p 5000:5000 re2pcap
```

OR

```
docker run --rm --cap-add NET_ADMIN -p 5000:5000 --name re2pcap amitraut/re2pcap
```

Open `localhost:5000` in your web browser to access Re2Pcap or use [Re2Pcap-cmd](https://github.com/Cisco-Talos/Re2Pcap/blob/master/Re2Pcap-cmd "Re2Pcap-cmd") script to interact with Re2Pcap [container](https://www.kitploit.com/search/label/Container "container") to get PCAP in current working directory  
  
**Requirements**

*   Docker
*   HTTP Raw Request / Response
*   Web Browser (for best results, please use **_Chromium_** based web browsers)

  
**Advantages**

*   Easy setup. No complex multi-VM setup required
*   Re2Pcap runs on Alpine Linux based docker image that weighs less than 100 MB :D
*   Allows you to dump simulated raw HTTP request and response in to PCAP

  
**Dockerfile**

```
FROM alpine  
  
# Get required dependencies and setup for Re2Pcap  
RUN echo "[http://dl-cdn.alpinelinux.org/alpine/edge/testing](http://dl-cdn.alpinelinux.org/alpine/edge/testing)" >> /etc/apk/repositories  
RUN apk update && apk add python3 tcpdump tcpreplay  
RUN pip3 install --upgrade pip  
RUN pip3 install pexpect flask requests httpretty requests-toolbelt  
  
COPY Re2Pcap/ /Re2Pcap  
RUN cd Re2Pcap && chmod +x Re2Pcap.py  
  
WORKDIR /Re2Pcap  
EXPOSE 5000/tcp  
  
# Run application at start of new container  
CMD ["/usr/bin/python3", "Re2Pcap.py"]
```

  
**Walkthrough**

*   Video walkthrough shows pcap creation for Sierra [Wireless](https://www.kitploit.com/search/label/Wireless "Wireless") AirLink ES450 ACEManager iplogging.cgi [command ](https://www.talosintelligence.com/reports/TALOS-2018-0746 "command ")[injection](https://www.kitploit.com/search/label/Injection "injection") vulnerability using Re2Pcap web interface

[![](https://1.bp.blogspot.com/-S7cPKgomrVU/XjorIAva53I/AAAAAAAARnQ/QCDfjDdLN7Q6lB-Z_0McnwevSjNwBe8CwCNcBGAsYHQ/s640/Re2Pcap_4_Re2Pcap_Demo.gif)](https://1.bp.blogspot.com/-S7cPKgomrVU/XjorIAva53I/AAAAAAAARnQ/QCDfjDdLN7Q6lB-Z_0McnwevSjNwBe8CwCNcBGAsYHQ/s1600/Re2Pcap_4_Re2Pcap_Demo.gif)

  

*   Video walkthrough of PCAP creation for Sierra Wireless AirLink ES450 ACEManager iplogging.cgi [command injection vulnerability](https://www.talosintelligence.com/reports/TALOS-2018-0746 "command injection vulnerability") using Re2Pcap-cmd script

[![](https://1.bp.blogspot.com/-Nv35pNRdS9E/XjorOCUCeSI/AAAAAAAARnU/TSNAr3yN1uozRGMw0ebz6uTmrKIhNNJiwCNcBGAsYHQ/s640/Re2Pcap_5_Re2Pcap_Demo1.gif)](https://1.bp.blogspot.com/-Nv35pNRdS9E/XjorOCUCeSI/AAAAAAAARnU/TSNAr3yN1uozRGMw0ebz6uTmrKIhNNJiwCNcBGAsYHQ/s1600/Re2Pcap_5_Re2Pcap_Demo1.gif)

  
**Re2Pcap Workflow**  

[![](https://1.bp.blogspot.com/-s1Zrrns-i1Q/XjorToXojdI/AAAAAAAARnc/heCjS3arKWQJ6JlKQI5Y2Rf1bbZTay6dgCNcBGAsYHQ/s640/Re2Pcap_6_workflow.png)](https://1.bp.blogspot.com/-s1Zrrns-i1Q/XjorToXojdI/AAAAAAAARnc/heCjS3arKWQJ6JlKQI5Y2Rf1bbZTay6dgCNcBGAsYHQ/s1600/Re2Pcap_6_workflow.png)

  
As shown in the above image Re2Pcap is Alpine Linux based Python3 application with Flask based web interface  
Re2Pcap parses the input data as raw HTTP request or response and actually perfoms client/server interaction while capturing packets. After the interaction Re2Pcap presents the captured packets as PCAP file  
  
**Recommendations**

*   Please use Linux as your host operating system as Re2Pcap is well tested on Linux
*   If creating PCAP for `Host: somedomain:5000` i.e. port 5000, please change Flask application to run on other port by modifying Re2Pcap.Py `app.run` call otherwise PCAP will contain Flask application response

  
**Limitations**

*    If raw HTTP request is without `Accept-Encoding:` header `Accept-Encoding: identity` is added in the reqeust  
    
    *   There is known [issue](https://github.com/psf/requests/issues/2234 "issue") for it in python requests. Following is closing note for that issue
    
    >  That's really fairly terrible. Accept-Encoding: identity is always valid, the RFCs say so. It should be utterly harmless to send it along. Otherwise, removing this requires us to replace httplib. That's a substantial bit of work. =(
    
*    The following are source and desination IPs in PCAPs from Re2Pcap  
    
    *   Sourece IP: 10.10.10.1
    *   Destination IP: 172.17.0.2 or (Re2Pcap Container's IP Address)
    
    Please use `tcprewrite -D` option to modify desitnation IP to something else as per your need. You may also use `tcpprep` and `tcprewrite` to set other IPs as endpoints. Due to inconsistent result of `tcprewrite` I used alternative way to set different SRC/DST IPs
*    Specifying `HTTP/1.1 302 FOUND` as response will generated PCAP with maximum possible retries to reach resource specified in `Location:` header. Plase export the first HTTP stream using [wireshark](https://www.kitploit.com/search/label/Wireshark "wireshark") in testing if you do not like the additional noise of other streams

  
  

**[Download Re2Pcap](http://whareotiv.com/oPS "Download Re2Pcap")**

**Regards**

**Kang Asu**