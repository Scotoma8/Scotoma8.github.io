---
layout: post
title: RetrieveBot资产信息收集与查询
subtitle: Shell Script [Under constant development]
bigimg: /img/path.jpg
tags: [Tools]
---

# [retrievebot](https://github.com/Scotoma8/retrievebot)
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
	
	./retrievebot -s
	[*] Usage : /usr/bin/retrievebot -s -Functionality(-i,-d,-p,-c,-w,-t,-r,-l) -h
	
	./retrievebot -m
	[*] Usage : /usr/bin/retrievebot -m -Functionality(-i,-d,-p,-c,-w,-t,-r,-l) -h
	
	./retrievebot -s -i
	[*] Single ip info script
	[*] Usage : /usr/bin/retrievebot -s -i <ip>
	
	./retrievebot -m -i
	[*] Multi ip info script
	[*] Usage : /usr/bin/retrievebot -m -i <file name of ips>