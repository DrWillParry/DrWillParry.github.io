---
date: "2024-04-01"
client: "Our Future Health"
title: "Developing a CSM system to monitor appointment quality"
author:
- Parry W
categories:
- Descriptive analysis
- Public health
- Monitoring systems
draft: false
published: N/A
---

## Summary

<a href="https://ourfuturehealth.org.uk/" target="_blank">Our Future Health</a> aims to be the UK's largest ever health research programme. It is designed to help everyone live longer and healthier lives through the discovery and testing of more effective approaches to prevention, earlier detection, and treatment of diseases.

Volunteers who sign up to take part attend an appointment at a clinic. At this appointment, they have blood samples taken and a range of point-of-care tests are conducted.

The aim of this project was to create a Central Statistical Monitoring system (CSM) which could be used for the ongoing quality monitoring of appointments. The software was developed using Snowflake as the DBMS, DBT to control data validation and processing, and Microsoft Power BI for development of the user interface and visualisations.

The monitoring solution provided a range of descriptive analyses of blood sample quality, point-of-care testing results and appointment completion measures. Statistical process control with covariate adjustment was used to identify whether any unusual appointment outcomes were associated with specific clinics in near-real time. The analyses are being used on an ongoing basis for targeting training to improve appointment quality.
