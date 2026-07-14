---
layout: page
title: Cross-Lingual Knowledge Consistency
description: Whether multilingual language models and public knowledge sources encode the same facts across languages — and what drives the gaps when they don't.
importance: 5
category: research
related_publications: true
---

Cross-lingual disagreement is the knowledge-translation diagnostic in its
purest form: only the language changes, yet the answers do too. This thread
studies whether multilingual language models and public knowledge sources
such as Wikipedia and Wikidata encode the same facts across languages, and
what drives the gaps when they don't.

[A Wikidata-Based Framework to Measure Cross-Lingual Bias in Multilingual
LLMs](/publications/#iferroudjene2026wikidata) (KG-LLM Workshop @ LREC 2026)
introduces **WILA-PopQA**, a popularity-matched multilingual benchmark
across 9 languages that disentangles three factors multilingual probing
benchmarks usually confound: the language of the question, the language of
the entity, and entity popularity. Across 12 open-weight LLMs, the language
of the question turns out to be the dominant factor, and matching it to the
entity's language does *not* reliably improve factual recall
{% cite iferroudjene2026wikidata %}.

The same question applies to the knowledge sources themselves:
[Factual Inconsistencies in Multilingual Wikipedia
Tables](/publications/#cappa2025factual) studies where the language
editions of Wikipedia disagree on structured facts, quantifying
inconsistencies that any model trained on this data inherits
{% cite cappa2025factual %}.
