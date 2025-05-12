---
title:  "Introduction to STPA Onto Converters"
categories: [Open Mic Session, Open Mic]
excerpt: "There are multiple tools which create structured STPA data. In this talk, we discuss a prototype tool which allows to convert STPA and System Control Structure (SCS) to the STPA ontology."
---

<!-- Fixing content of this file:
  - [IF NOT RUNNING FROM GITHUB ACTION] replace all variables within this file surrounded by `${` `}`, example values are:
    - OPEN_MIC_SESSION_TITLE=`Debugging SPARQL queries`
    - OPEN_MIC_SESSION_DATE=`Friday 4 April 2023`
  - remove all comments from this file
-->

On Friday 25 April 2025 [Bogdan Kostov](https://kbss.felk.cvut.cz/web/team#bogdan-kostov) held an Open Mic session with the topic \"Introduction to STPA Onto Converters\". Video and presentation included.

{% include video id="R44x5fuN_3w" provider="youtube" %}

##### Abstract
Systems Approach to Process Hazard Analysis (STPA) [[1](https://psas.scripts.mit.edu/home/wp-content/uploads/2016/01/Systems-Theoretic-Process-Analysis-STPA-John-Thomas.pdf),[2](http://psas.scripts.mit.edu/home/materials/)] is a modern, top-down, general hazard analysis method. It focuses on examining loss scenarios initiated or not avoided by the performance of control actions or lack there of. Typically in a practical environment after conducting an STPA analysis, the output will be further used in various different ways, e.g. create an analysis report for the management team, combined the output with outputs from other analysis. To ensure interoperability between tools which allow the export of STPA artifacts in various structured formats there must be:
1) a common format 
2) a tool to convert between different STPA formats to the common format.

This open mic session will present the STPA Onto Converters project [3] which aims to ensure interoperability between tools producing and consuming STPA artifacts. The project implements a set of automated converters which transform between various STPA formats and the STPA ontology which acts as the common format. 

**Outline** 
1) introduction STPA and the STPA ontology
2) STPA Onto Converters project and implemented converters
3) Future work

The presentation slides are available [at this link](https://docs.google.com/presentation/d/1yD5FeJULknTM2CPux54KGIAHlJbuCvxkaWcAdbanUG8/edit?usp=drive_link).

Further reading:

* [1] [STPA handbook](https://psas.scripts.mit.edu/home/wp-content/uploads/2016/01/Systems-Theoretic-Process-Analysis-STPA-John-Thomas.pdf). Leveson, Nancy G. & Thomas, J. P. MIT Partnership for Systems * Approaches to Safety and Security (PSASS), Cambridge, Massachusetts, U.S., 2018.
* [2] [STAMP Materials](http://psas.scripts.mit.edu/home/materials/), online, accessed 4.2025
* [3] [STPA Onto Converters](https://github.com/kbss-cvut/stpa-onto-converters), online , accessed 4.2025
