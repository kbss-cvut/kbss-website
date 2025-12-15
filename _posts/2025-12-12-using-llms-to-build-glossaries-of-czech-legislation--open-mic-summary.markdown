---
title: "Using LLMs to build glossaries of Czech legislation"
categories: [ Open Mic Session, Open Mic ]
excerpt: "We discuss how LLMs can be used to automate extraction of SKOS glossaries from Czech legislation documents."
---


On Friday 12 December 2025 [Martin Ledvinka](https://kbss.felk.cvut.cz/web/team#martin-ledvinka) held an Open Mic
session with the topic \"Using LLMs to build glossaries of Czech legislation.\"

{% include video id="fwu6Nz4GhIs" provider="youtube" %}

##### Abstract

Glossaries allow disambiguation of the meaning of words in a given context by creating _terms_ - pairs of label and
definition describing the label's semantics in a given context. However, creating such glossaries manually is an arduous
and time-consuming process. In this talk, experiments with using LLMs to extract glossaries from Czech
legislative documents were presented.

The approach builds a pipeline of downloading legislative documents, pre-processing them and then using a LLM to
extract a glossary of terms explicitly defined by the document. The output is then post-processed and
a [SKOS](https://www.w3.org/TR/skos-reference/) glossary
is created. Finally, the glossary can be imported to [TermIt](https://kbss-cvut.github.io/termit-web/) - a
terminological manager developed by the KBSS.

{% include figure image_path="assets/images/posts/2025-12-12-llm-pipeline.png" alt="Visualization of the
glossary-building pipeline" %}

While the steps of the proof-of-concept of the pipeline are to a large extent manual, they have great potential for
automation, and the output of this pipeline can be used as a seed for creating more complex glossaries that include also
terms defined implicitly by the document.

The presentation slides are
available [at this link](https://docs.google.com/presentation/d/1LcXMLDop0O06gK7EJh_5YrE7TkJfZ6AzbZKjEgxr19Y/edit?usp=sharing).

Further reading:

* [SKOS](https://www.w3.org/TR/skos-reference/)
* [TermIt: Managing normative thesauri](https://journals.sagepub.com/doi/10.3233/SW-243547)
* [Semantic Vocabulary of Terms](https://datagov-cz.github.io/ssp/) (Czech only)
