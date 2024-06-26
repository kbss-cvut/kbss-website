---
title: "Open Mic - Refactoring Application Ontology Concepts in JOPA based Applications"
categories: [Open Mic Announcement, Open Mic]
---

On Thursday 11th April 2024, our speaker [Bogdan Kostov](https://kbss.felk.cvut.cz/web/team#bogdan-kostov) had a presentation about refactoring ontolgies, mainly its concepts, in JOPA based applications.

{% include video id="d1lfWU4b4es" provider="youtube" %}

TODO: add description of the real presentation

Renaming application ontology concepts leads to refactoring of JOPA (Java OWL Persistence API) based application. In this context application ontology is defined as a formal artifact, for example represented in OWL[2]/RDF[3] specifying the schema of application data. JOPA is a Java framework for ontology based data access to OWL storage systems, such as triple stores. JOPA's main data access method is read and write JOPA entities, i.e. java classes mapped to application ontology concepts. Renaming application ontology concepts requires further refactoring of affected JOPA application artifacts. For example JOPA entities as well as data. This talk will explore practical guidelines and methods to support the identification and refactoring of application artifacts affected by the renamed application ontology concepts in a JOPA based client-server application.

Further reading:
1. [JOPA - Java OWL Persistence API](https://github.com/kbss-cvut/jopa)
1. [Web Ontology Language (OWL)](https://www.w3.org/OWL/)
1. [Resource Description Framework (RDF)](https://www.w3.org/RDF/)
