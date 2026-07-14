---
layout: page
title: Research
permalink: /research/
nav: true
nav_order: 3
---

### Toward a Science of Knowledge Translation

My research studies what happens at the boundaries between different representations of knowledge — text, tables, knowledge graphs, queries, logical formulas, and language model parameters. Moving between these forms is never lossless, and whether two representations encode the same knowledge depends on what population, time frame, or scope is assumed. Expressing the same knowledge in multiple forms and studying where the versions disagree is a diagnostic: it tells us what each representation captures, what it silently drops, and where context is doing hidden work.

Turning this diagnostic stance into predictive theory: when is a mapping
between representations faithful, what does it silently drop, and can
representational loss be measured rather than merely observed? The
long-term goal is knowing in advance which kinds of knowledge survive
which translations.

<figure style="margin: 2rem 0;">
  <svg
    viewBox="0 0 920 640"
    role="img"
    aria-label="The research program as a graph. Nodes are representations of knowledge: natural language, knowledge graphs, formal logic, SQL and relational schemas, and language model parameters. Labeled edges are research threads, colored by pillar. First pillar, between language models and knowledge graphs: knowledge base construction maps language model parameters to knowledge graphs; cross-lingual consistency maps natural language to natural language; GraphRAG maps knowledge graphs to natural language. Second pillar, from language to logic: autoformalization maps natural language to formal logic; temporal knowledge maps between natural language and knowledge graphs with time qualification. Third pillar, applied translation: text-to-SQL maps natural language to SQL; UNIFIED, a domain instance, maps clinical records to clinical vocabularies."
    style="width: 100%; height: auto; font-family: inherit;"
  >
    <defs>
      <marker id="arrow-p1" viewBox="0 0 10 10" refX="9" refY="5" markerWidth="7" markerHeight="7" orient="auto-start-reverse">
        <path d="M 0 0 L 10 5 L 0 10 z" fill="var(--global-theme-color)"></path>
      </marker>
      <marker id="arrow-p2" viewBox="0 0 10 10" refX="9" refY="5" markerWidth="7" markerHeight="7" orient="auto-start-reverse">
        <path d="M 0 0 L 10 5 L 0 10 z" fill="#2698ba"></path>
      </marker>
      <marker id="arrow-p3" viewBox="0 0 10 10" refX="9" refY="5" markerWidth="7" markerHeight="7" orient="auto-start-reverse">
        <path d="M 0 0 L 10 5 L 0 10 z" fill="#42b983"></path>
      </marker>
    </defs>

    <!-- Pillar 1: between language models and knowledge graphs -->
    <a href="#between-language-models-and-knowledge-graphs">
      <path d="M 470 78 C 560 100, 620 110, 672 118" fill="none" stroke="var(--global-theme-color)" stroke-width="2" marker-end="url(#arrow-p1)"></path>
      <text x="565" y="88" text-anchor="middle" font-size="15" fill="var(--global-theme-color)">KBC</text>
    </a>
    <a href="#between-language-models-and-knowledge-graphs">
      <path d="M 100 240 C 40 190, 130 175, 165 238" fill="none" stroke="var(--global-theme-color)" stroke-width="2" marker-start="url(#arrow-p1)" marker-end="url(#arrow-p1)"></path>
      <text x="112" y="172" text-anchor="middle" font-size="15" fill="var(--global-theme-color)">cross-lingual</text>
    </a>
    <a href="#between-language-models-and-knowledge-graphs">
      <path d="M 648 176 C 540 230, 400 258, 262 270" fill="none" stroke="var(--global-theme-color)" stroke-width="2" marker-end="url(#arrow-p1)"></path>
      <text x="470" y="219" text-anchor="middle" font-size="15" fill="var(--global-theme-color)">GraphRAG</text>
    </a>

    <!-- Pillar 2: from language to logic -->
    <a href="#from-language-to-logic">
      <path d="M 155 290 L 155 466" fill="none" stroke="#2698ba" stroke-width="2" marker-end="url(#arrow-p2)"></path>
      <text x="168" y="385" font-size="15" fill="#2698ba">autoformalization</text>
    </a>
    <a href="#from-language-to-logic">
      <path d="M 258 244 C 420 190, 540 165, 636 148" fill="none" stroke="#2698ba" stroke-width="2" marker-start="url(#arrow-p2)" marker-end="url(#arrow-p2)"></path>
      <text x="445" y="166" text-anchor="middle" font-size="15" fill="#2698ba">temporal (time-qualified)</text>
    </a>

    <!-- Pillar 3: applied translation -->
    <a href="#applied-translation-official-statistics-and-digital-health">
      <path d="M 258 286 C 420 330, 530 360, 618 390" fill="none" stroke="#42b983" stroke-width="2" marker-end="url(#arrow-p3)"></path>
      <text x="435" y="322" text-anchor="middle" font-size="15" fill="#42b983">text-to-SQL</text>
    </a>

    <!-- nodes -->
    <g>
      <rect x="330" y="30" width="190" height="48" rx="10" fill="var(--global-card-bg-color, var(--global-bg-color))" stroke="var(--global-divider-color)" stroke-width="1.5"></rect>
      <text x="425" y="59" text-anchor="middle" font-size="16" fill="var(--global-text-color)">LM parameters</text>
    </g>
    <g>
      <rect x="640" y="120" width="215" height="48" rx="10" fill="var(--global-card-bg-color, var(--global-bg-color))" stroke="var(--global-divider-color)" stroke-width="1.5"></rect>
      <text x="747" y="149" text-anchor="middle" font-size="16" fill="var(--global-text-color)">knowledge graphs</text>
    </g>
    <g>
      <rect x="60" y="240" width="198" height="48" rx="10" fill="var(--global-card-bg-color, var(--global-bg-color))" stroke="var(--global-divider-color)" stroke-width="1.5"></rect>
      <text x="159" y="269" text-anchor="middle" font-size="16" fill="var(--global-text-color)">natural language</text>
    </g>
    <g>
      <rect x="80" y="470" width="150" height="48" rx="10" fill="var(--global-card-bg-color, var(--global-bg-color))" stroke="var(--global-divider-color)" stroke-width="1.5"></rect>
      <text x="155" y="499" text-anchor="middle" font-size="16" fill="var(--global-text-color)">formal logic</text>
    </g>
    <g>
      <rect x="618" y="380" width="240" height="48" rx="10" fill="var(--global-card-bg-color, var(--global-bg-color))" stroke="var(--global-divider-color)" stroke-width="1.5"></rect>
      <text x="738" y="409" text-anchor="middle" font-size="16" fill="var(--global-text-color)">SQL / relational schemas</text>
    </g>

    <!-- UNIFIED domain instance (pillar 3) -->
    <g>
      <rect x="310" y="500" width="500" height="110" rx="12" fill="none" stroke="var(--global-divider-color)" stroke-width="1.5" stroke-dasharray="6 5"></rect>
      <text x="330" y="524" font-size="13" fill="var(--global-text-color-light, var(--global-text-color))">domain instance</text>
      <rect x="335" y="540" width="150" height="42" rx="8" fill="var(--global-card-bg-color, var(--global-bg-color))" stroke="var(--global-divider-color)" stroke-width="1.5"></rect>
      <text x="410" y="566" text-anchor="middle" font-size="14" fill="var(--global-text-color)">clinical records</text>
      <a href="#applied-translation-official-statistics-and-digital-health">
        <path d="M 490 561 L 578 561" fill="none" stroke="#42b983" stroke-width="2" marker-end="url(#arrow-p3)"></path>
        <text x="534" y="551" text-anchor="middle" font-size="14" fill="#42b983">UNIFIED</text>
      </a>
      <rect x="585" y="540" width="200" height="42" rx="8" fill="var(--global-card-bg-color, var(--global-bg-color))" stroke="var(--global-divider-color)" stroke-width="1.5"></rect>
      <text x="685" y="566" text-anchor="middle" font-size="14" fill="var(--global-text-color)">clinical vocabularies</text>
    </g>
  </svg>
  <figcaption style="font-size: 0.875rem; color: var(--global-text-color-light); margin-top: 0.5rem;">
    The research program, drawn as what it is — a graph. Nodes are representations of knowledge; labeled edges are the research threads that map one into another, colored by pillar (each edge links to its pillar below).
  </figcaption>
</figure>

The three pillars below each work a bundle of these edges.

### Between Language Models and Knowledge Graphs

What do language models actually know, and how does it line up with what
knowledge graphs state? This pillar works the interface in all three
directions: extraction, consistency, and injection.

**Knowledge base construction from language models.** Treating LLMs as
compressed, implicit knowledge bases — extracting and evaluating their
factual content, and comparing it to structured sources such as Wikidata.

**Cross-lingual knowledge consistency.** Whether multilingual models and
public knowledge sources such as Wikipedia and Wikidata encode the same
facts across languages — and what drives the gaps when they don't.
Cross-lingual disagreement is the diagnostic in its purest form: only the
language changes, yet the answers do too. WILA-PopQA (KG-LLM Workshop @
LREC 2026) disentangles question language, entity language, and entity
popularity, showing that the language of the question dominates factual
recall.

**Retrieval-augmented generation with knowledge graphs.** Using structured
knowledge to ground retrieval and generation — from KG-based passage
expansion for question answering to mapping the fast-growing GraphRAG
landscape. RAG is knowledge translation at inference time: what the graph
contributes depends on how its structure is verbalized for the model.

Related projects:
[Knowledge Base Construction from Language Models](/projects/kbc-from-lms/) ·
[Cross-Lingual Knowledge Consistency](/projects/cross-lingual-consistency/)

### From Language to Logic

**Autoformalization and deductive reasoning.** Translating
natural-language statements into formal representations (logic, queries)
and studying how LLMs perform deductive reasoning once knowledge is made
explicit.

**Temporal knowledge and reasoning.** Time is where knowledge translation
fails hardest: texts underspecify validity intervals, knowledge graphs
qualify them, and language models flatten them into timeless facts.
ChronoSense (ACL 2025) evaluates interval-based temporal understanding via
Allen relations, exposing gaps between knowing *when* events happened and
reasoning about how they relate.

Related projects:
[Autoformalization and Deductive Reasoning](/projects/autoformalization/)

### Applied Translation: Official Statistics and Digital Health

**Text-to-SQL over real-world statistical data.** Working with Statistics
Netherlands (CBS) on translating natural-language questions into SQL over
complex statistical tables, where schema design encodes implicit context
about populations and time frames. Home of the
[LOCuST benchmark](https://lagewel001.github.io/LOCuST/): 2,244 real
statistical tables across 22 domains, 2,567 annotated questions, in
English and Dutch.

**Semantic harmonisation in digital health (UNIFIED).** Knowledge
translation under regulatory constraint: harmonising patient-centred
endpoints across devices, studies, and clinical vocabularies — the domain
where translation loss has clinical consequences. Data integration and
semantic harmonisation for patient-centred clinical-study endpoints
derived from digital health technologies, as part of the EU Innovative
Health Initiative project UNIFIED.

Related projects:
[Text-to-SQL over Real-World Statistical Data](/projects/text-to-sql-statistics/) ·
[Semantic Harmonisation in Digital Health (UNIFIED)](/projects/unified/)
