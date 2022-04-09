# Cybersecurity for Developers / CODELEX 
 
| Contact | Data |
|---------| ------ |
| e-mail  | m.akermanis@gmail.com |

## Intro

This relatively short course will cover some key elements on how to secure your code.

Most of the web app 'hacking' courses put main effort on teaching how to break applications.
That approach is all fine, but such a broad subject cannot realistically be covered in 6 sessions.

So - in order to squeeze as much information as possible in our sessions, some of the 'hottest' topics will be discussed in greater detail (including practical exercises), while for some further research must be done by students themselves. 

It's organized in following sections (on some sessions we could cover multiple topics, while some others could take more time):

- OWASP Top 10 (2021) vulnerabilities:
  - [ ]  A01:2021-Broken Access Control
  - [ ]  A02:2021-Cryptographic Failures
  - [ ]  A03:2021-Injection
  - [ ]  A04:2021-Insecure Design
  - [ ]  A05:2021-Security Misconfiguration
  - [ ]  A06:2021-Vulnerable and Outdated Components 
  - [ ]  A07:2021-Identification and Authentication Failures
  - [ ]  A08:2021-Software and Data Integrity Failures
  - [ ]  A09:2021-Security Logging and Monitoring Failures
  - [ ]  A10:2021-Server-Side Request Forgery
- Some additional stuff:
  - [ ]  Risks of 3rd party code libraries
  - [ ]  API security
  - [ ]  Brief coverage of network attacks
- ✨ Some more magic if we have time left ✨

## What's the plan
As mentioned previously - not everything can be fully covered in such a brief timespan, so we will have to adapt and improvise. 

Meaning - as much as possible practical demos will be done in sessions, leaving most of the student assignments as homeworks.

Assignments involving the challenges will be marked with 👾 symbol.\
The more 👾👾👾, the harder it should be (but of course, depends on your previous experience on subject).

## Requirements

**Basic understanding of how web application works and interacts with different services:**

- [HTTP basics](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP)
- [HTTP GET/POST requests and headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/Session)
- [Basic JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
- [Basic SQL](https://www.dataquest.io/blog/sql-basics/)
- [HTTP cookies](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies)
- [Cross-Origin Resource Sharing (CORS)](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)
- [Application program interface (API)](https://www.techtarget.com/searchapparchitecture/definition/RESTful-API)
- [Basic cryptography (SSL/TLS)](https://developer.mozilla.org/en-US/docs/Web/Security/Transport_Layer_Security)
- [Linux cli basics](https://ubuntu.com/tutorials/command-line-for-beginners#3-opening-a-terminal)
- [We will not have much time to play around with scripting, but Python is fun :)](https://www.w3schools.com/python/python_intro.asp)

## How to get ready for the 1st session:

1. **Install a virtualization hypervisor software on your PC. That way we will be able to have guest OS inside host OS:**

</br>Choose from one of these:
- [VirtualBox] - Easy to install/use virtualization software (Win/macOS/Linux)
- [VMware Player] - VMware Windows software (Win/macOS - called VMware Fusion/Linux)

    *If you are already using a Linux, theoretically you can skip this and install all the tools manually, but anyway VM is a way to go in case you break something (just revert from Snapshot and keep hacking).

2. **Install a Linux OS as a Virtual Machine in any of aforementioned software. Since everybody knows that it's quite hard to do 'hacking' on Windows, we need some kind of Linux OS to get most of the tools working:**

</br>Choose from one of these:
  - [Kali Linux] - Most widely used Linux distro for cyber-sec
  - [Parrot OS] - Same features as Kali, so just a matter of preference

3. **Install Docker, so we can run vulnerable web apps inside the Docker containers**:
 * [Install instructions](https://docs.docker.com/engine/install/debian/)
 
4. **Install the Juice Shop web application as a Docker container, so we have a 'real-life' web app running - will have demos and practice done there:**
- [Juice Shop] - Intentionally vulnerable AngularJS based web application.  [Install instructions](/01/resources/juice_shop_install.md)\
[+] Other vulnerable web apps could be used later in the course, but if needed we will install them later.

5. **Get ready to intercept HTTP requests (Kali linux should come with Burp Suite pre-installed, but please double-check):**
- [Burp Suite Community Edition] - An integrated platform/graphical tool for performing security testing of web applications
- [FoxyProxy Standard] - A firefox browser extension to quickly switch between browser proxy settings 

6. **Deploy the Juice Shop application, run it and complete these steps**
   - Thoroughly explore the web application (walk the "Happy Path" as this will make your life easier on solving the challenges). </br>Make mental notes on: 
     1) Content
     2) Functionality
     3) Paths
     4) User roles
     5) Any files/documents hosted
     6) GET/POST request parameters
     7) Request headers
     8) Entry points for user input
     9) Tech stack and 3rd party components (like code libraries) used
   - Register yourself as a new user
   - *👾* Find a way to access the ScoreBoard page of the web app
   
[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [Kali Linux]: <https://www.kali.org/get-kali/>
   [Parrot OS]: <https://parrotsec.org/docs/download-parrot.html>
   [VirtualBox]: <https://www.virtualbox.org/wiki/Downloads>
   [VMware Player]: <https://www.vmware.com/se/products/workstation-player/workstation-player-evaluation.html>
   [Juice Shop]: <https://owasp.org/www-project-juice-shop/>
   [Burp Suite Community Edition]: <https://portswigger.net/burp/documentation/desktop/getting-started>
   [FoxyProxy Standard]: <https://addons.mozilla.org/en-US/firefox/addon/foxyproxy-standard/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search>
