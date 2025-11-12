---
title:  "Exploring Ontology Engineering Workflow with TermIt and Other Tools"
categories: [Open Mic Session, Open Mic]
excerpt: "Short description of the session topic that is displayed below the article header on the landing page."
---

<!-- Fixing content of this file:
  - [IF NOT RUNNING FROM GITHUB ACTION] replace all variables within this file surrounded by `${` `}`, example values are:
    - OPEN_MIC_SESSION_TITLE=`Debugging SPARQL queries`
    - OPEN_MIC_SESSION_DATE=`Friday 4 April 2023`
  - remove all comments from this file
-->

On Friday 31 October 2025 [Bogdan Kostov](https://kbss.felk.cvut.cz/web/team#bogdan-kostov) held an Open Mic session with the topic \"Exploring Ontology Engineering Workflow with TermIt and Other Tools\". Video and presentation included.

{% include video id="-UriTtvcnmE" provider="youtube" %}

##### Abstract

This session presents evaluation of using TermIt in the process of building a domain/application ontology based on a corpus of domain specific text. The motivation behind this using TermIt is to improve collaboration between domain experts and ontology engineers. TermIt allows easy term definition and semi-automated text annotation, features which allow domain experts to define terms and their usage in a text corpus. To continue the ontology engineering process, e.g., formalizing concepts and testing, defined domain terms and annotated text corpus in TermIt has to be exported and processed. For example defined terms can be extracted in an ontology file compatible with Protégé where terms can be formally described and organized in a taxonomy. Annotated texts can be extracted and can be used for verification and validation, e.g., how many of the terms occur in the text corpus, fetch occurrences of a particular term to compare with the text and formal based definitions. 

Experiences using TermIt in this scenario are discussed. This includes challenges importing and exporting ontologies and text documents into and from TermIt as well as limitations of TermIt vocabulary management and text annotation features. 

The examples in this session are mainly based on a case study building an airport safety domain ontology using TermIt.

The presentation slides are available [at this link](https://docs.google.com/presentation/d/1rKaHDldbp1F3pGre0CgfmpFjr8VmL7UGtj6XDeSswA8/edit?usp=drive_link).


Further reading:
* [SABiO: Systematic approach for building ontologies](https://www.researchgate.net/publication/286670309_SABiO_Systematic_approach_for_building_ontologies)
* [TermIt](https://github.com/kbss-cvut/termit-ui)
* [Protégé](https://protege.stanford.edu/)
* [SKOS Simple Knowledge Organization System](https://www.w3.org/TR/skos-reference/)
* [Resource Description Framework RDF](https://www.w3.org/RDF/)
* [SPARQL](https://www.w3.org/TR/sparql11-query/)
* [OWL](https://www.w3.org/OWL/)