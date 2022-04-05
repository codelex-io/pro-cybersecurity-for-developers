# Cybersec_4_Devs
Cybersecurity for Developers / CODELEX 

## Intro

This short course will cover some key elements on how to secure your code.

Most of the 'hacking' courses put main effort on teaching how to break application.
Such approach is all fine, but such a broad subject cannot realistically be covered in 6 sessions.

So - in order to squeeze as much information as possible in our sessions, some of 'hottest' topics will be discussed in greater detail (including practical exercises), while some will have be explained and additional research should be done by students themselves. 

It's organized in following sections (on some sessions we could cover multiple topics, while some others could more time):

- OWASP Top 10 (2021) vulnerabilities:
    - A01:2021-Broken Access Control
    - A02:2021-Cryptographic Failures
    - A03:2021-Injection
    - A04:2021-Insecure Design
    - A05:2021-Security Misconfiguration
    - A06:2021-Vulnerable and Outdated Components 
    - A07:2021-Identification and Authentication Failures
    - A08:2021-Software and Data Integrity Failures
    - A09:2021-Security Logging and Monitoring Failures
    - A10:2021-Server-Side Request Forgery
- Mapping the application
- Risks of 3rd party code libraries
- Brief coverage of network attacks
- ✨ Some more magik ✨

## What is the plan
As mentioned previously - everything cannot be fully covered in such a brief time, so we will have to adapt and improvise. Meaning - as much practical demo will be done as possible, leaving most of the student assignments as homeworks

## Requirements

Basic understanding of how web application works and interacts with different services:

- HTTP GET/POST requests and headers
- Basic JS
- Basic SQL
- Session handling
- APIs
- Basic web cryptography, like SSL/TLS
- We will not have much time to play around with scripting, but Python is fun :)

## ToDo

1. Since everybody knows that it's quite hard to do 'hacking' on Windows, we need some kind of Linux OS to get most of the tools working. You can choose from these two Debian based distros:
- [Kali Linux] - Most widely used Linux distro for cybersec
- [Parrot OS] - Same features as Kali, so just a matter of prefference

2. You can install the Linux OS as a Virtual Machine on your host PC using any of these tools:

- [VirtualBox] - Easy to install/use virtualization software (Win/MacOS/Linux)
- [VMWare Player] - VMWare Windows software (Win/MacOS (called VMWare Fusion)/Linux)

*If you are already using a Linux, technically you can skip this and install all the tools manually, but anyway VM is a way to go in case you break something (just revert from Snapshot and keep hacking).

3. Install the Juice Shop web application locally, so we have a 'real-life' web app running - there we will have demos and practice done:
- [Juice Shop] - Intentionally vulnerable AngularJS based web application (I would prefer to run it as a Docker container, but choose for yourself).
- Other vulnerable web apps could be used later in the course, but if needed we will install them later.

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [Kali Linux]: <https://www.kali.org/get-kali/>
   [Parrot OS]: <https://parrotsec.org/docs/download-parrot.html>
   [VirtualBox]: <https://www.virtualbox.org/wiki/Downloads>
   [VMWare Player]: <https://www.vmware.com/se/products/workstation-player/workstation-player-evaluation.html>
