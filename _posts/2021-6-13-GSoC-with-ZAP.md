---
layout: post
title: GSoC 2021 with OWASP ZAP
---
![GSoC ZAP Banner](/images/GSoC-ZAP-banner.png)

Hello everyone!   
I'm excited to share with all of you that this summer I'll be working on adding Retest functionality to ZAP as a part of my Google Summer of Code 2021 project, under the guidance of my mentors Simon([psiinon](https://github.com/psiinon)), Rick([kingthorin](https://github.com/kingthorin)), and Ricardo([thc202](https://github.com/thc202)). This is the first of a series of posts that I'll use to document my progress as I go along.

ZAP is the world's most widely used web app scanner for DAST(Dynamic Application Security Testing). You can learn more about ZAP over [here](https://www.zaproxy.org/) and can follow [@zaproxy](https://twitter.com/zaproxy) on Twitter for the latest ZAP updates.

While ZAP is a great tool for testing for vulnerabilities of various types in web applications and generating alerts accordingly, it still currently lacks a user-friendly mechanism to retest identified vulnerabilites. With this project, I'll be aiming to add this to ZAP with the help of a Retest add-on, which will allow users to specify alerts which they want to be retested, and leave the task of setting up the scan settings accordingly to ZAP. Once implemented, there are a couple of ways in which this addon could be used, which are listed below :-

* #### **Using the ZAP Desktop** - The user can select specific alerts they wish to retest by selecting them in the Alerts Tab, or via clicking on the retest menu option and choosing the required alerts from the Retest dialog that appears(they can filter the alerts on the basis of the sites). They can choose to then click on retest and see the retest results in the dialog itself, or they can click on the "Generate Retest Plan" button in order to generate a retest plan, which could be used in the future. They can also load a previous retest plan from the retest dialog via the use of the "Load Retest Plan" button. Note that a retest plan can only be generated when the session is in memory, and that once a session is persisted, the alerts present in the session cant be retested anymore. However,a stretch goal of my project would be to allow the generation of retest plans from saved sessions as well.

* #### **Using the command line** - The user can also automate the retesting of alerts via the use of the [Automation Framework](https://www.zaproxy.org/docs/desktop/addons/automation-framework/), by simply using the retest plan as the configuration file to be provided to the -autorun option.

There are loads of other ways in which the add on could be used(using it as a __test__ metric for known vulnerable applications), but those will have to wait until the core part of the addon is successfully implemented.

I'm definitely looking forward to a great summer implementing this, and I hope to share as much of it with you as I can :)
