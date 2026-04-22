---
layout: page
title: Autoformalization and Deductive Reasoning
description: Translating natural-language statements into formal representations, and studying where LLMs succeed and fail once knowledge is made explicit.
img: assets/img/projects/chronosense.png
importance: 1
category: research
related_publications: true
---

Formal representations promise precision and verifiability, but only if the
translation from natural language is faithful. This thread studies where that
translation breaks down — in deductive reasoning, in temporal reasoning, and
in the general problem of converting human statements into logic, programs,
or structured queries.

Our ECAI 2025 paper [Investigating the Robustness of Deductive Reasoning with
Large Language Models](/publications/#hoppe2025investigating) tests how small
prompt and input variations affect deductive reasoning, characterises common
failure modes, and proposes an evaluation setup for robustness. Our ACL 2025
paper [ChronoSense](/publications/#islakoglu2025chronosense) examines
temporal understanding using Allen-style event intervals, highlighting
current gaps in interval reasoning. Ongoing supervision work extends this
line to GRPO-based autoformalization from natural language to first-order
logic.
