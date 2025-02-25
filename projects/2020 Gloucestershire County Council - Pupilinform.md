---
date: "2020-03-27"
client: "Gloucestershire County Council"
title: "Pupilinform online data analysis tool"
author:
- Parry W
- Marden R
categories:
- Education policy
- Monitoring systems
draft: false
published: N/A
---


## Summary

<img src="/image/logo.png" alt="Pupilinform logo" width="200"/>

Gloucestershire County Council wanted to build an online data analysis tool for their pupil wellbeing survey. This tool would be accessed by authorised teachers and stakeholders to conduct *ad hoc* analysis of the survey answers. The tool needed to:

* be highly secure, with robust password-protected access
* allow for a variety of pre-specified *and* *ad hoc* analyses
* provide a variety of granularity to outputs dependent on user role (school, council, etc.)
* allow for secure and appropriately censored data download
* allow visualisation outputs to be downloadable as Word reports
* be accessible to up to 400 users whilst remaining on budget

A tool was developed using the following software:

* AWS EC2 was used to host the application
* Auth0 was used to control user authorisation
* ShinyProxy was used to containerise the application
* R Shiny was used to develop the application
