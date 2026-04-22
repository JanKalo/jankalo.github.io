---
layout: page
title: Knowledge Base Construction from Language Models
description: Treating LLMs as compressed, implicit knowledge bases — extracting, evaluating, and comparing their knowledge to structured sources.
importance: 2
category: research
related_publications: true
---

A large language model is a compressed, implicit knowledge base. This thread
asks what kind of knowledge base it is — how to extract it, how to evaluate
it, and where it diverges from structured sources like Wikidata.

Methodological work includes [KAMEL](/publications/#kalo2022kamel) (AKBC 2022),
a probing benchmark with multi-token entities;
[Evaluating the Knowledge Base Completion Potential of GPT](/publications/#veseli2023evaluating)
(EMNLP Findings 2023), a systematic study of LLMs as KB completion sources;
and [KnowlyBERT](/publications/#kalo2020knowlybert) (ISWC 2020), a hybrid
architecture combining language models with knowledge graphs at query time.
Earlier work on [Prompt Tuning or Fine-Tuning](/publications/#fichtel2021prompt)
(AKBC 2021) and [Prompting as Probing](/publications/#alivanistos2022prompting)
(LM-KBC 2022) laid the groundwork for treating LMs as queryable KBs. The
position paper [Large Language Models and Knowledge Graphs: Opportunities and
Challenges](/publications/#pan2023large) (TGDK 2023) maps the broader space.

Recent work extends this to multilingual settings:
[A Wikidata-Based Framework to Measure Cross-Lingual Bias in Multilingual
LLMs](/publications/#iferroudjene2026wikidata) (KG-LLM @ LREC 2026) introduces
the WILA-PopQA benchmark and disentangles the effects of question language,
entity language, and popularity on factual recall.

I co-organise the [LM-KBC Challenge](https://lm-kbc.github.io/) at ISWC,
which has run since 2022.
