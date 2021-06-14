---
layout: post
title: GSoC 2021 with OWASP ZAP
---
![GSoC ZAP Banner](/images/GSoC-ZAP-banner.png)

Hello everyone!   
I'm excited to share with all of you that this summer I'll be working on adding Retest functionality to ZAP as a part of my Google Summer of Code 2021 project, under the guidance of my mentors Simon([psiinon](https://github.com/psiinon)), Rick([kingthorin](https://github.com/kingthorin)), and Ricardo([thc202](https://github.com/thc202)).  

ZAP is the world's most widely used web app scanner for DAST(Dynamic Application Security Testing). You can learn more about ZAP over [here](https://www.zaproxy.org/) and can follow [@zaproxy](https://twitter.com/zaproxy) on Twitter for the latest ZAP updates.

While ZAP is a great tool for testing for vulnerabilities of various types in web applications and generating alerts accordingly, it still currently lacks a user-friendly mechanism to retest identified vulnerabilites. With this project, I'll be aiming to add this to ZAP with the help of a Retest add-on, which will allow users to specify alerts which they want to be retested, and leave the task of setting up the scan settings accordingly to ZAP. Once implemented, there are a few ways in which this addon could be used, which are listed below :-

* Using the ZAP Desktop - The user
  
