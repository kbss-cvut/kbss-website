---
title: "Publishing RDF metadata in dedicated catalogues"
categories: [ Open Mic Summary, Open Mic ]
excerpt: "Showcase of a metadata management and publishing environment Piveau in the context of need for publishing and metadata discovery environment for scientific metadata described by DCAT based metadata profiles."
---

On Friday 9th January 2026 at 10:30 [Michal Med](https://kbss.felk.cvut.cz/web/team#michal-med) talked about effective publishing of RDF based metadata (based on RDF top level vocabularies for metadata description, such as SKOS, Dublin Core, DCAT etc.).

{% include video id="KxzXAqyGTGo" provider="youtube" %}

##### Problem definition

The current approach to research data leads to the need for a catalogue solution, which will be able to consume RDF-based metadata regardless of its nature - whether it is a book, a map, a manuscript, material data observation, or a chemical experiment protocol. In [one of the previous open mic sessions](https://kbss.felk.cvut.cz/web/publishing-open-science-metadata-open-mic-summary) we have introduced Czech Core Metadata Model -- a DCAT extension metadata profile designed to describe common properties of research data with possibility to be exteded for the needs of specific scientifiec fields.

{% include figure image_path="./assets/images/posts/2026-01-09-research-data-jungle.png" alt="Research data jungle" %}

But as the researchers provide the metadata in RDF based serializations of CCMM and DCAT(-AP), there is still a need to catalogize the metadata in RDF based catalogue, that allows to use the capabilites of RDF approach, such as searching the domain specific metadata properties. Many 'catalogues' are now based on the dataset repositories (!), that flatten the graph metadata model and are then very uneffective in discovery, searching and statistical dashboards. 

The problem may be defined as looking for effective way to publish machine readable metadata in a catalogue that allows lossless discovery of all relevant information for various purposes, from finding relevant data to overall statistics about published data, creating dashboards and reusing and interconnecting data.

##### Piveau catalogue as an solution

Tha basic assumption is that data are properly described with metadata based on concepts from top level metadata ontologies, such as SKOS[1], Dublin Core[2], DCAT[3] etc. This is something that is already taken into account in the process of creation of metadata profiles. But it is also important to publish metadata using the catalogues that allow users to fully utilize the benefits of using graph metadata.

In this talk we took a specific data management ecosystem called piveau[4] as a metadata catalogue for publishing and harvesting metadata from various providers. This tool is used (among others) as a metadata catalogue for european data portals and is between possibel candidates to be used in building of Czech node of European Open Science Cloud [5] as a metadata management tool and catalogue.

The talk described the multilevel architecture of the environment, consisting of storage part (Hub), harvesting part (Consus) and validation and reporting tools (Metrics). In the practical part it is shown how to create catalogue, import metadata or harvest them from remote catalogue. Piveau is based on Virtuoso triple store and DCAT based metadata profiles, allows user management using Keycloak and indexing in Elasticsearch. Typical flor starts with original resources, harvesting them, analysing and discovering them and reusing them in other tools, such as statistical dashboards. Most of the tools are using UI only for end users, catalogue and metadata management is usually done using API, described in piveau hub-repo service.

Related links:

1. [SKOS](https://www.w3.org/TR/skos-reference/)
1. [Dublin Core](https://www.dublincore.org/)
1. [Data Catalog Vovabulary (DCAT) Version 3](https://www.piveau.de/en/)
1. [piveau](https://www.piveau.de/en/)
1. [EOSC CZ](https://www.eosc.cz/)
