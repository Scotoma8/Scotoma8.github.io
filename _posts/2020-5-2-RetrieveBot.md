---
layout: post
title: RetrieveBot - Info Gathering&Querying
subtitle: Shell Script
bigimg: /img/path.jpg
tags: [Red-Team]
---

**工具简介:**   

# retrievebot [under constant development]
Asset Information Collecting and Quering.

Author:Scotoma8   
Disclaimer:   
&emsp;&emsp;This tool was developed from the kali platform and used only for education purpose or authorized situations.   
&emsp;&emsp;Any illegal use has nothing to do with the author.

Usage:

	./retrievebot -h
	[*] RetrieveBot - A Tool of Asset Information Collecting
	[*] There're two modes for this tool:
	[*]     -s mode:quering for single target.
	[*]     -m mode:quering for multiple targets and the param needs to be a file.
	[*] Functionality:
	[*]     -h:help messages.
	[*]     -i:quering ip infomation.
	[*]     -d:quering domain name's ip resolving infomation.
	[*]     -p:quering port information.
	[*]     -c:quering subdomain information.
	[*]     -w:quering whois information of ip or domain name.
	[*]     -t:quering whatweb information of ip or domain name.
	[*]     -r:quering subdirs information of url.
	[*]     -l:crawling words and email addresses of url.
	[*]     -e:requesting domain name through HTTP&HTTPS [WORKING IN -m MODE].
	
	./retrievebot -s
	[*] Usage : /usr/bin/retrievebot -s -Functionality(-i,-d,-p,-c,-w,-t,-r,-l) -h
	
	./retrievebot -m
	[*] Usage : /usr/bin/retrievebot -m -Functionality(-i,-d,-p,-c,-w,-t,-r,-l,-e) -h
	
	./retrievebot -s -i
	[*] Single ip info script
	[*] Usage : /usr/bin/retrievebot -s -i <ip>
	
	./retrievebot -m -i
	[*] Multi ip info script
	[*] Usage : /usr/bin/retrievebot -m -i <file name of ips>
	
	./retrievebot -m -e
	[*] Multi domain request script
	[*] Usage : /usr/bin/retrievebot -m -e <file name of domains>

Issue:   	

	a).proxychains + nmap result in segmentation fault:   
	1.export http_proxy and https_proxy   
	2.use proxychains-ng   
	sudo apt-get install git gcc   
	sudo apt-get remove proxychains   
	git clone https://github.com/rofl0r/proxychains-ng.git   
	cd proxychains-ng/   
	./configure --prefix=/usr --sysconfdir=/etc   
	make   
	sudo make install   
	sudo make install-config   
	
	b).dirb use export http_proxy result in error - unsupported socks:   
	1.use proxychains or proxychains-ng   


​	
