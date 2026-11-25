---
title: "Upcoming Open Mic - Czech Core Metadata Model: From Specification to Metadata"
categories: [Open Mic Announcement, Open Mic]
excerpt: "We present the Czech Core Metadata Model for research datasets, the tooling around it, and what still gets lost on the way to published metadata."
---

On Friday 27 November 2026 at 11:30 [Michal Med](https://kbss.felk.cvut.cz/web/team#michal-med) is going to
talk about the Czech Core Metadata Model (CCMM) and what it takes to get from a metadata specification to
metadata that are actually published.
Join the session at [this link](https://meet.jit.si/open-mic-kbss).

##### Abstract

The Czech Core Metadata Model (CCMM) is a metadata model for describing research datasets in the Czech
national open science infrastructure. It was developed by the EOSC CZ Metadata Working Group and builds on DCAT
and DataCite. Its new version 2.0.0 was released this autumn. The talk follows the structure of a journal paper
we are currently writing about it.

We start with the motivation and design principles of the model, and show how the specification is maintained in
Dataspecer. We then look at the tooling around it: transforming XML instances into RDF/XML, Turtle and JSON-LD,
and checking that all serializations say the same thing. A plain text comparison does not work for that, because
each serialization orders triples differently and gives blank nodes different labels. So we canonicalize the graphs
first, using the W3C RDF Dataset Canonicalization algorithm (RDFC-1.0). It gives every blank node a stable label and
writes the triples as sorted N-Quads. When two graphs are equivalent, their canonical forms are identical, so they
can be compared line by line. Finally, we discuss what does not work yet. Publishing metadata through
InvenioRDM, and therefore DataCite, loses information. The gaps against DCAT-AP 3 are handled by mappings rather
than by changes to the model. We end with an open question for discussion: is it time for an RDF-native metadata catalogue?


###### Further reading:
* [CCMM on GitHub](https://github.com/techlib/CCMM)
* [Dataspecer on GitHub](https://github.com/mff-uk/dataspecer)
* [RDF Dataset Canonicalization (RDFC-1.0)](https://www.w3.org/TR/rdf-canon/)
