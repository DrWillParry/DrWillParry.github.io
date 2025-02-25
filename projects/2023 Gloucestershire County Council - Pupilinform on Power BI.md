---
date: "2023-03-27"
date-format: MMM YYYY
title: "Moving the Pupilinform online data analysis tool to Power BI"
author:
- Parry W
categories:
- Exploratory analysis
- Education policy
- Research report
- Monitoring systems
draft: false
published: (awaiting permission)
published-title: Date
abstract: "Gloucestershire County Council"
abstract-title: Client
---

<!---
## Links

* <a href="https://bmjopen.bmj.com/content/13/11/e075152" target="_blank">Journal article</a>
--->

## Introduction

This report documents the findings of the proof-of-concept (POC) work for Gloucestershire County Council (GCC) on whether a replacement to Pupilinform – the pupil wellbeing survey analysis tool – can be built using Power BI. It aims to provide an initial understanding of whether it is possible to replicate Pupilinform on Power BI, and if so, identify the elements that are straightforward, those that are difficult, and those that may not be possible. It is not exhaustive, as there may be several ways in which to accomplish some elements, and it does not aim to fully duplicate all of the functionality of Pupilinform exactly. However, it should provide a sound basis on which to make decisions regarding the use of Power BI to replace the current version of Pupilinform, and provide some indication of the effort required to complete a first beta version.


## Summary and conclusions

The POC work was challenging and resulted in both good solutions and limitations in transferring Pupilinform to Power BI. Much of the core functionality of Power BI is possible to replicate using Power BI, but there are some key gaps and issues that need to be considered.

Core functionality that could be incorporated included:

1. controlling filtering and cross-tabulation of data using table joins and slicers,
2. producing the correct data summarisations and passing them to visuals so that plots could be constructed,
3. controlling the data that users can pass to the visuals, using row-level security, slicer values, and role-specific versions of the reports, and
4. creating the same plots as available in Pupilinform using R script visuals.

Core functionality that could not be incorporated included:

1. the suppression of small counts (beyond simply hiding values <5) to prevent the possibility of back-calculation from the remaining values and totals in table visuals,
2. a straightforward method of creating downloadable reports that are correctly formatted, and
3. incorporation of the mean WEMWBS score in the Summary plots.

For the suppression of small counts, it may be worth seeing whether a DAX expert may be able to incorporate improved suppression rules into the table visuals used for data download.

There were also some limitations it is possible to work around:

1. enforced phase filtering for specific (Ofsted) Summary topics,
2. squashing and stretching of plots dependent on the amount of data being displayed, and
3. correct sorting of questions and values in visuals and tables.

There was also one other important consideration that relates to:

1. the way in which users access Power BI from external organisations and any costs associated with this. Power BI subscriptions may need to be paid unless GCC can add external users to its organisational Power BI user groups.

Ultimately, the POC work has been very successful in prototyping solutions for moving Pupilinform onto the Power BI platform. GCC will need to carefully consider the limitations that have been identified. It may be necessary for GCC to undertake additional work on these before a final decision can be made and work can begin on building a Power BI-based solution for release to users.