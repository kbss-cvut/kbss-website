---
title:  "LLM-Powered Coder Assistants"
categories: [Open Mic Session, Open Mic]
excerpt: "Code-generating LLMs are powerful pattern matchers, not magic. This session breaks down how they transform prompts into working code using transformers, attention, and tokenization. We'll dive into their training process, common pitfalls like hallucinations and biases."
---

On Friday 23 May 2025 Evgenii Grigorev held an Open Mic session with the topic \"LLM-Powered Coder Assistants\". Video and presentation included.


{% include video id="3uEKVppwo1g" provider="youtube" %}

##### Abstract

Code-generating LLMs are not wizards — they’re sophisticated pattern matchers trained on terabytes of code. But how do they turn a prompt like "Sort this CSV by date and calculate weekly averages" into working Python? This session will demystify the :

* Core mechanics -- Transformers, attention layers, and tokenization
* Training secrets: From GitHub scrapes to context-aware fine-tuning.
* Why they fail: Hallucinations, hidden biases, and the "copy-paste paradox".
* Examples from data analysis (Pandas, SQL) will illustrate key concepts.

**Outline**

1. Introduction to LLMs: Transformers, tokenization, and the "autocomplete on steroids" paradigm.

2. Tools Deep Dive: GitHub Copilot, ChatGPT, CodeWhisperer, and open-source alternatives (StarCoder, Llama 3).

3. Under the Hood: Training on GitHub data, context window limitations, and safety guardrails.

4. Pros vs. Cons: 55% faster coding (GitHub study) vs. 40% of generated code containing vulnerabilities (Stanford research).

The presentation slides are available [at this link](https://drive.google.com/drive/folders/1av8p5QM3ebM4V2lX9csUB7TXRpWNt27e?usp=sharing).

Further reading:
* [Attention Is All You Need](https://arxiv.org/abs/1706.03762)
* [Evaluating Large Language Models Trained on Code](https://arxiv.org/abs/2107.03374)
