---
title:  "Data extraction from Czech Register of Contracts"
categories: [Open Mic Session, Open Mic]
excerpt: "An overview of the Czech Register of Contracts and our experience with extracting a relational model from the text of its contracts."
---

On Friday 23 October 2026 [Miroslav Blaško](https://kbss.felk.cvut.cz/web/team#miroslav-blaško) held an Open Mic session with the topic \"Data extraction from Czech Register of Contracts\".

{% include video id="j1J-IbLZiaM" provider="youtube" %}

The recording is also available [on YouTube](https://youtube.com/live/j1J-IbLZiaM).

##### Abstract

The talk presented the first step towards knowledge-based question answering over the [Czech Register of Contracts](https://smlouvy.gov.cz), which consists mostly of PDF documents: understanding the corpus and extracting a relational model from the text of the contracts, demonstrated on the use case of a reinsurance company assessing risks in forestry.

###### Understanding the corpus

Czech public bodies must publish every contract over CZK 50,000 excl. VAT. Its metadata are structured but incomplete, and the values that matter, such as prices, volumes and places, are only in the attachments. The talk showed the contracts of the state forest enterprise Lesy České republiky: 130,213 contracts with 150,421 attachments, 99.8% of them PDFs (1.26 million pages; only 0.8% of the PDFs need OCR). 85.6% of the contracts state their value and 22.5% amend another contract. Since then, the corpus has grown to 12 forest and nature-conservation publishers (e.g. Vojenské lesy a statky ČR, national park administrations, city forests of Prague and Brno) with 217,847 contracts.

###### The tool

We developed a tool that turns the contracts of any publisher, given its company ID, into a relational database. It downloads the metadata and attachments, converts the PDFs to Markdown with page markers (MuPDF) and splits the metadata into seven normalised tables, including chains of amendments. Two domain-specific steps follow: regular expressions over the subject of each contract assign activity categories (e.g. 47,886 timber sales), and a language model (qwen3.8-27b) reads the wanted values from the text. A JSON schema makes the model back every value with a verbatim quote, a page number and a confidence, and each quote is checked against the text.

{% include figure image_path="assets/images/posts/2026-10-23-register-of-contracts-pipeline.png" alt="The five steps of the extraction pipeline: download records, convert to Markdown, export metadata, classify records, extract model" %}

###### Extraction results

The model read 33,033 contracts selling timber or harvesting rights and found the volume in 72% of them, the price in 49% and the forest district in 92%; 95–99% of its quotes are verbatim in the text. Volume × price matches the amount in the register within 2% for 99.4% of 15,597 contracts.

###### Future work

Next, we plan text-to-SQL and (Graph)RAG question answering over the tables, linking the contracts with geodata, and research on the extraction itself: a taxonomy of errors, an ontological description of attributes and cross-checks as a free gold dataset.

The presentation slides are available [at this link](https://drive.google.com/file/d/1bZ6BEJP-f9peoLf1iesyiTWYHujiQ4vf/view?usp=sharing).

###### Further reading:
* [Registr smluv](https://smlouvy.gov.cz) – the register's portal
* [Open data of the register](https://data.smlouvy.gov.cz) – monthly XML dumps
* [Hlídač státu](https://www.hlidacstatu.cz/) – independent portal with full-text search
