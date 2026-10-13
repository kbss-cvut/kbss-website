---
title: "Upcoming Open Mic - Data extraction from Czech Register of Contracts "
categories: [Open Mic Announcement, Open Mic]
---


The Open mic session starts on Friday 16th October 2026 at 10:30 via [this link](https://meet.jit.si/open-mic-kbss). [Miroslav Blaško](https://kbss.felk.cvut.cz/web/team#miroslav-blaško) is going to talk about own tools and techniques to extract data from Czech Regiter of Contracts (Registr smluv).

##### Abstract

The Czech Register of Contracts (Registr smluv) is a public registry where Czech public-sector bodies must publish their contracts worth more than CZK 50,000. It is a rich source of information on public spending, but most of it is locked in PDFs. Since July 2016, the register has collected almost 10 million records (contract versions). Their metadata (parties, subject, value, dates, amendments) is structured, but the numbers that matter, such as prices, quantities and places, are only in the attachments.

As part of a research project, we are developing a tool that extracts data from the register into a relational database. On top of it, we plan to build text-to-SQL question answering over the contracts, supported by a knowledge base that describes the database schema. In the talk, I will describe the characteristics of this dataset and the techniques we use to extract data from it. I will also demonstrate the current state of the tool: for a selected set of contracts (e.g. all contracts of one organisation), it downloads metadata and attachments, converts PDFs to Markdown, normalises the metadata into tables, classifies the contracts by activity, and extracts values with a language model, each backed by a verbatim quote and page number.


The presentation 

###### Further reading:
* [Registr smluv](https://smlouvy.gov.cz) – the register's portal
* [Open data of the register](https://data.smlouvy.gov.cz) – monthly XML dumps
* [Hlídač státu](https://www.hlidacstatu.cz/) – independent portal with full-text search over the register
