---
title: "Upcoming Open Mic - Publishing Open Science metadata"
categories: [Open Mic Announcement, Open Mic]
---


<!-- Naming convention: post MUST be named beginning with YEAR-MM-DD-title.MARKDOWN. Create a COPY of this file in _posts and rename it according to the convention. The date is not date of presentation, but date of publication of the announcement. The title in human readable form is put in the quotes to the title parameter in front matter  -->
<!-- Fixing content of this file:
  - [IF NOT RUNNING FROM GITHUB ACTION] replace all variables within this file surrounded by `${` `}`, example values are:
    - OPEN_MIC_SESSION_TITLE=`Debugging SPARQL queries`
    - OPEN_MIC_SESSION_DATE=`Friday 4 April 2023`
  - remove all comments from this file
-->
The Open mic session starts on Friday 10 October 2025 at 10:30 via [this link](https://meet.jit.si/open-mic-kbss). [Michal Med](https://kbss.felk.cvut.cz/web/team#michal-med) presents outputs of his work on metadata profile for Czech cell of European Open Science Cloud.

{% include figure image_path="/assets/images/openmics/2025-10-10-eosc.png" alt="Czech cell of EOSC %}{: .align-right .profile-photo}

##### Abstract

The objective of the European Open Science Cloud (EOSC)[1] is to provide researchers and innovators in Europe with an open and trusted multi-disciplinary environment where they can publish, find and reuse data, tools and services for research and innovation. Through this environment, EOSC aims to mobilise, align and scale resources across Europe to accelerate open science, higher productivity and increased reproducibility and trust in research.

Organization behind the implenmentation is EOSC Federation and as it usually is, federation is gathered from the national cells. The goals are iplemented mainly on the national structure. One of the main goals is development of multidisciplnary data repository to allow researchers publish their data in accordance with FAIR principles [2] (Findable, Accessible, Interoperable and Reusable). It seems that only way to publish it this way is to set up metadata catalogue and describe data using newly created interoperable metadata profile.

This profile called Czech Core Metadaa Model for Research Data[7] was created in 1st half of 2025 in cooperation with National Technical Library and CESNET based on widely used metadata profiles DataCite[3], Dublin Core[4] and DCAT[5] using tool DataSpecer[6], that was already presented in Open Mic.

Currently it is being implemented in National Metadata Directory (NMA) and Catch-all repository of EOSC project. This talk describes the creation of the profile and possible problems with its implementation.

Further reading:
1. [European Open Science Cloud](https://research-and-innovation.ec.europa.eu/strategy/strategy-research-and-innovation/our-digital-future/open-science/european-open-science-cloud-eosc_en)
2. [FAIR Principles](https://www.go-fair.org/fair-principles/)
3. [Data Cite](https://datacite-metadata-schema.readthedocs.io/en/4.6/)
4. [Dublin Core](https://www.dublincore.org/)
5. [DCAT](https://www.w3.org/TR/vocab-dcat-3/)
6. [DataSpecer](https://dataspecer.com/)
7. [Czech Core Metadata Model for Research Data](https://model.ccmm.cz/research-data/en/)
