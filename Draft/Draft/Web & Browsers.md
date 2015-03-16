##Web, Web Applications & Browsers

[Bypassing WAFs](http://www.nethemba.com/bypassing-waf.pdf)

https://xss-game.appspot.com/

XSS game http://escape.alf.nu/








[leaps - shared text editing in Golang](https://github.com/denji/leaps)
* Leaps is a service for hosting collaboratively edited documents using operational transforms to ensure zero-collision synchronization across any number of editing clients.



[Postcards from a Post-XSS World - Michael Zalewski](http://lcamtuf.coredump.cx/postxss/#dangling-markup-injection)
* This page is a rough collection of notes on some of the fundamental alternatives to direct script injection that would be available to attackers following the universal deployment of CSP or other security mechanisms designed to prevent the execution of unauthorized scripts. I hope to demonstrate that in many cases, the capabilities offered by these alternative methods are highly compatible with the goals of contemporary XSS attacks. 

[Drupal Attack Scripts](https://github.com/gfoss/attacking-drupal)
* Set of brute force scripts and Checklist

[Drupal Security Checklist](https://github.com/gfoss/attacking-drupal/blob/master/presentation/drupal-security-checklist.pdf)

[SQL Injection wiki](http://www.sqlinjectionwiki.com/)

[Shadow Daemon](https://shadowd.zecure.org/overview/introduction/)
* Shadow Daemon is a collection of tools to detect, protocol and prevent attacks on web applications. Technically speaking, Shadow Daemon is a web application firewall that intercepts requests and filters out malicious parameters. It is a modular system that separates web application, analysis and interface to increase security, flexibility and expandability. Shadow Daemon is free software. It is released under the license GPLv2, so its source code can be examined, modified and distributed by everyone.

[unindexed](https://github.com/mroth/unindexed/blob/master/README.md)
* The site is constantly searching for itself in Google, over and over and over, 24 hours a day. The instant it finds itself in Google search results, the site will instantaneously and irrevocably securely delete itself. Visitors can contribute to the public content of the site, these contributions will also be destroyed when the site deletes itself.



[Self-Exfiltration: The Dangers of Browser-Enforced Information Flow Control](http://ericchen.me/self_exfiltration.pdf)
* Abstract �Since the early days of Netscape, browser vendors and web security researchers have restricted out-going data based on its destination. The security argument accompanying these mechanisms is that they prevent sensitive user data from being sent to the attacker�s domain. However, in this paper, we show that regulating web information flow based on its destination server is an inherently flawed security practice. It is vulnerable to self-exfiltration attacks, where an adversary stashes stolen information in the database of a whitelisted site, then later independently connects to the whitelisted site to retrieve the information. We describe eight existing browser security mechanisms that are vulnerable to these �self-exfiltration� attacks. Furthermore, we discovered at least one exfiltration channel for each of the Alexa top 100 websites. None of the existing information flow control mechanisms we surveyed are sufficient to protect data from being leaked to the attacker. Our goal is to prevent browser vendors and researchers from falling into this trap by designing more systems that are vulnerable to self-exfiltration.


[The Devil is in the Constants: Bypassing Defenses in Browser JIT Engines](http://users.ics.forth.gr/~elathan/papers/ndss15.pdf)
* Abstract �Return-oriented programming (ROP) has become the dominant form of vulnerability exploitation in both user and kernel space. Many defenses against ROP exploits exist, which can significantly raise the bar against attackers. Although protecting existing code, such as applications and the kernel, might be possible, taking countermeasures against dynamic code, i.e., code that is generated only at run-time, is much harder. Attackers have already started exploiting Just-in-Time (JIT) engines, available in all modern browsers, to introduce their (shell)code (either native code or re-usable gadgets) during JIT compilation, and then taking advantage of it. Recognizing this immediate threat, browser vendors started employing defenses for hardening their JIT engines. In this paper, we show that�no matter the employed defenses�JIT engines are still exploitable using solely dynamically generated gadgets. We demonstrate that dynamic ROP payload construction is possible in two modern web browsers without using any of the available gadgets contained in the browser binary or linked libraries. First, we exploit an open source JIT engine (Mozilla Firefox) by feeding it malicious JavaScript, which once processed generates all re- quired gadgets for running any shellcode successfully. Second, we exploit a proprietary JIT engine, the one in the 64-bit Microsoft Internet Explorer, which employs many undocumented, specially crafted defenses against JIT exploitation. We manage to bypass all of them and create the required gadgets for running any shellcode successfully. All defensive techniques are documented in this paper to assist other researchers. Furthermore, besides showing how to construct ROP gadgets on-the-fly, we also show how to discover them on-the-fly, rendering current randomization schemes ineffective. Finally, we perform an analysis of the most important defense currently employed, namely constant blinding , which shields all three-byte or larger immediate values in the JIT buffer for hindering the construction of ROP gadgets. Our analysis suggests that extending constant blinding to all immediate values (i.e., shielding 1-byte and 2-byte constants) dramatically decreases the JIT engine�s performance, introducing up to 80% additional instructions



###Securing Web Applications


[Center for Internet Security Apache Server 2.4 Hardening Guide](https://benchmarks.cisecurity.org/tools2/apache/CIS_Apache_HTTP_Server_2.4_Benchmark_v1.1.0.pdf)



[Magical Code Injection Rainbow Framework](https://github.com/SpiderLabs/MCIR)
* The Magical Code Injection Rainbow! MCIR is a framework for building configurable vulnerability testbeds. MCIR is also a collection of configurable vulnerability testbeds. Has testing lessons for xss/csrf/sql



###LFI & RFI

[LFI Local File Inclusion Techniques (paper)](http://www.ush.it/2008/08/18/lfi2rce-local-file-inclusion-to-remote-code-execution-advanced-exploitation-proc-shortcuts/) 
* This paper exposes the ability from the attacker standpoint to use /proc in order to exploit LFI (Local File Inclusion) vulnerabilities. While using /proc for such aim is well known this one is a specific technique that was not been previously published as far as we know. A tool to automatically exploit LFI using the shown approach is released accordingly. 
* [Update: a third (known) technique has been dissected here](http://www_ush_it/2008/07/09/local-file-inclusion-lfi-of-session-files-to-root-escalation/ ) 


[Liffy](https://github.com/rotlogix/liffy)
* Liffy is a Local File Inclusion Exploitation tool. 
Current features include: 
data:// for code execution
expect:// for code execution
input:// for code execution
filter:// for arbitrary file reads
/proc/self/environ for code execution in CGI mode
Apache access.log poisoning
Linux auth.log SSH poisoning
Direct payload delivery with no stager
Support for absolute and relative paths 
Support for cookies
! I have had issues with access log poisoning on current versions of Apache. This not an issue with the payload delivery and or poisoning. This is more of an issue with the request after the poisoning to kick off your shell. This may require a browser refresh. 









###HTML 5


[SH5ARK](http://sh5ark.professionallyevil.com)
* The Securing HTML5 Assessment Resource Kit, or SH5ARK, is an open source project that provides a repository of HTML5 features, proof-of-concept attack code, and filtering rules. The purpose of this project is to provide a single repository that can be used to collect sample code of vulnerable HTML5 features, actual attack code, and filtering rules to help prevent attacks and abuse of these features. The intent of the project is to bring awareness to the opportunities that HTML5 is providing for attackers, to help identify these attacks, and provide measures for preventing them

* [Presentation on SH5ARK](https://www.youtube.com/watch?v=1ZZ-vIwmWx4)

* [GetSH5ARK here](http://sourceforge.net/projects/sh5ark/)




##(NO)SQL Injection


[SQL Injection Cheat Sheet](http://ferruh.mavituna.com/sql-injection-cheatsheet-oku/)


[SQL Injection Knowledge Base](http://websec.ca/kb/sql_injection#MySQL_Testing_Injection)

[Pen Testing MongoDB](http://www.irongeek.com/i.php?page=videos/derbycon4/t408-making-mongo-cry-attacking-nosql-for-pen-testers-russell-butturini)

[Laduanum](http://laudanum.sourceforge.net/)
* �Laudanum is a collection of injectable files, designed to be used in a pentest when SQL injection flaws are found and are in multiple languages for different environments.They provide functionality such as shell, DNS query, LDAP retrieval and others.�








SQLi Lab lessons
From: https://github.com/Audi-1/sqli-labs
SQLI-LABS is a platform to learn SQLI Following labs are covered for GET and POST scenarios: 
Error Based Injections (Union Select) 
String
Integer
Error Based Injections (Double Injection Based)
BLIND Injections: 1.Boolian Based 2.Time Based
Update Query Injection.
Insert Query Injections.
Header Injections. 1.Referer based. 2.UserAgent based. 3.Cookie based.
Second Order Injections
Bypassing WAF 
Bypassing Blacklist filters Stripping comments Stripping OR & AND Stripping SPACES and COMMENTS Stripping UNION & SELECT
Impidence mismatch
Bypass addslashes()
Bypassing mysql_real_escape_string. (under special conditions)
Stacked SQL injections.
Secondary channel extraction