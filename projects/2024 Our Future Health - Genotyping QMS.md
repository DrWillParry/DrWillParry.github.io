---
date: "2024-08-01"
date-format: MMM YYYY
title: "Developing a genotyping Quality Monitoring System (QMS)"
author:
- Parry W
- Arathimos R
- Ponting L
categories:
- Descriptive analysis
- Public health
- Monitoring systems
draft: false
published: N/A
published-title: Date
abstract: Our Future Health
abstract-title: Client
---

## Summary

<a href="https://ourfuturehealth.org.uk/" target="_blank">Our Future Health</a> aims to be the UK's largest ever health research programme. It is designed to help everyone live longer and healthier lives through the discovery and testing of more effective approaches to prevention, earlier detection, and treatment of diseases.

Volunteers who sign up to take part attend an appointment at a clinic. At this appointment, they have blood samples taken which are then genotyped.

The aim of this project was to create a Quality Monitoring System (QMS) which could be used for the ongoing quality monitoring of the genotyping process. The software was developed using Snowflake as the DBMS, DBT to control data validation and processing, and Microsoft Power BI for development of the user interface and visualisations.

The monitoring solution provided a range of descriptive analyses of genotyping quality measures, for example:

* monitoring of both sample plates and resulting beadchip arrays
* identifying whether call rates met the required threshold
* successful sex identification and comparison with self-report
* target gene amplification (TGA) control probe values within recommended range
* ensuring technical replicate and control samples met concordance criteria
* identifying whether certain locations on beadchips/plates were associated with failure rates

More information on the Our Future Health genotyping process is available here:
<a href = "https://ourfuturehealth.gitbook.io/our-future-health/data/genotype-array-data" target = "_blank">https://ourfuturehealth.gitbook.io/our-future-health/data/genotype-array-data</a>


