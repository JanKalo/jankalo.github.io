---
layout: page
title: Text-to-SQL over Real-World Statistical Data
description: Natural-language interfaces to official statistical data, in collaboration with Statistics Netherlands (CBS). Home of the LOCuST benchmark.
importance: 3
category: research
---

Statistical databases are a uniquely hard testbed for natural-language
interfaces. Schemas encode implicit context about populations, time frames,
and inclusion rules, and a syntactically valid query can return a
statistically meaningless number without any visible error. This thread
studies text-to-SQL on real statistical data, in ongoing collaboration with
Statistics Netherlands (CBS).

A central output of this work is **LOCuST**, a multilingual benchmark for
text-to-SQL over official statistical data. LOCuST pairs natural-language
questions with a complex relational schema and a knowledge-graph component
that carries table- and measure-level metadata (labels, definitions, units,
hierarchical relations). The benchmark supports fine-grained evaluation via
an obsF1 metric that decomposes into measure and dimension components,
making it possible to study *where* errors arise rather than only whether
the final query is correct.

Work on and around LOCuST investigates several open questions: the
cost-performance trade-off between large reasoning models, small models,
and agentic refinement loops; what kinds of KG metadata actually help a
model link questions to schema elements; and — perhaps most importantly —
how to detect *unanswerability* and silent failure, where a query executes
but returns a number that is statistically meaningless because the context
(population, temporal scope, valid joins) was silently dropped in
translation.
