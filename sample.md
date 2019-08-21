# Google Summer of Code 2019 - OWASP (Final Submission)

## Table of Contents

- Overview
    - About me
    - Project details
    - Proposed summary
    - Work done

- Contributions
    - Pull requests
        - Detailed view in Google docs (with links to the PR)
        - Minimal view in Google spreadsheet (with links to the PR)
        - View here
    - Commits
    - Contributions graph and status

- Blog posts made

- Screenshots, screenscasts and tutorial videos

- Future work

- Personal experience and journey

- Conclusion

## Overview
### Project details

The OWASP SecureTea Project focuses on providing a one-stop security solution for various devices (personal computers / servers / IoT devices).

Currently the following features are supported:

- [x] Intrusion Detection System
- [x] Firewall
- [x] AntiVirus
- [x] Server Log Monitor
- [x] System Log Monitor
- [x] Local Web Deface Detection & Prevention System
- [x] Auto Web Server Patcher
- [x] IoT Anonymity checker
- [x] Auto report generation using OSINT
- [x] Notifying suspicious activities using various mediums (Twitter, Telegram, Slack, Gmail, SMS, AWS & more)
- [x] Interactive GUI for ease of setting up

Project URL: https://www.github.com/OWASP/SecureTea-Project
IRC channel: link

### Proposed summary

**Proposed summary as per proposal**:

Laying down a strong foundation & base architecture for Intrusion detection & prevention system (IDS/IPS), intelligent log monitoring, antivirus that can be scaled in future and also can be further expanded easily by applying machine learning. Enhance the current firewall by bringing in some advanced rules to detect malformed & suspicious packets & dump them into a PCAP file for future forensic analysis. Implement OSINT tools to collect information about attackers and generate a CSV report. Introduce Auto Server patcher to patch server configuration for maximum security features and implement a server side web deface detection. Also, protect IoT devices by checking if they are under the Shodan radar. Perform all the elemental connections & introduce different modes for the user. Improve the GUI by adding all the configurations options and critical data such as last login to it. Perform bug fixes and improve the dashboard. Write a detailed documentation and readme, and finally package and ship SecureTea version 1.1 on PyPi.

### Work done

Summary of the work done during the GSoC Phase (I - III):
"""This needs detailed Improvement."""

- Implemented Intrusion Detection System capable of detecting R2L attacks and reconnaissance attacks
- Introduced advanced packet filter rules for Firewall
- Introduced PCAP dumping of rejected packets for future forensic analysis
- Implemented System Log Monitor capable of detecting un-authorized system manipulation and attacks
- Implemented Server Log Monitor capable of processing Apache & Nginx log files to detect web attacks
- Implemented AntiVirus by using signature scanning and incorporating other open source antivirus for heruistic scanning
- Introduced SecureTea Auto Server Patcher to patch system and server configurations for maximum security features & overcome common deployment mistakes
- Implemented Local web deface detection & prevention mechanism
- Brought intelligence to Firewall by making it learn bad IPs from Intrusion Detection System, System Log Monitor, Server Log Monitor
- Introduced auto detail collection of hackers using the bad IPs as collected by IDS, Firewall, System log Monitor, Server Log Monitor using Open Source intelligence tools
- Introduced IoT Anonymity checker to protect IoT devices
- Performed elemental connections of elements & introduced 3 modes (server, system and IoT)
- Performed front-end Angular JS task
- Last logins
- Deployed on Heroku
- Protect using HTTPS
- Packaging
- Performed bug fixes
- Documentation - User guide & developer guide
- Raised relevant issues

## Contributions
### Pull requests
#### View here


## Future Work

The followings are the projected milestone for the next release:

- Testing project on various Linux flavours
- Peforming bug fixes
- Extending support to different Linux distributions
- Using SecureTea as a service instead of a python package
- Packaging on `.deb` , `.rpm` Linux packages

Long roadmap:
- Improving the current features
- Adding more features
    - SecureTea browser plugin: A plugin which can scan for harmful URL, monitor every URL, detect phishing sites & restrict internet activity.
    - Real-time log visualization & monitoring dashboard - If plotted in a graph with the right metrics, they can give back so vitalinformation just by looking. And plotting them realtime? ​ We are catching a thief red-handed​ , that’s quite cool! We can use Plotly to build this, it’s much more easy to integrate with a Flask app.
    - Enhance AntiVirus
      a. Behavioural​ based:
          i. Bring machine learning to detect and predict malware using Portable Executable(PE) headers​ .
          ii. Analyze the behaviour of a file by looking at its ​ API call​, it’s h​ooks with the Kernel​, it’s startup​, ​ system calls​ & TCP connections by using machine & deep learning.
          iii. Convolutional neural networks ​ (CNN)​ for ​ malware visualization​ .
      b. Integrate volatility​ to perform m emory malware​ analysis.
        i. Catching memory malware is one of the toughest thing out there, catching it will advance our anti-virus even more.
"""edit here."""

## Personal experience and journey

Can't beleive it's been 8 months since I started contributing to OWASP. Time flies by so fast. I remember the first contribution I made to SecureTea-Project was a simple correction in the setup packaging & some readme typos. Since then I progressed to understand the code base at a more deeper leve l and started sending some core patches and that was it.

It's been an amazing journey so far. I can say my learning graph has shown an exponential growth. I have learned a lot during the last 3-4 months. I understood the importacne of unit-tests and testing in general, understood that software is not only about coding, but a lot goes in maintaining a decent documentation and providing an intuitive version of software to the users for a satisfying user experience. Earlier, I considered tests as a waste of time and effort, use that time to impelement a new feature or improve the current. I was wrong at many levels! As our codebase continued to grow, I understood testing keeps the code intact without you worrying about the regression when adding or a modifying a feature.

GSoC changed my view towards software engineering, following a certain prototype model, planning and discussing before implementing anything is crucial for a good software development. It's not only about coding, regular testing and regular beta releases are very important.

I personally learnt a lot from my mentor, @rejahrehim. He's been really supportive throughout the journey.
