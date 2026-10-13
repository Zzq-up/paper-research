# Research Method Guide

## 1. Literature Search Planning

For each research question, record:

- Research question
- Core concepts
- Synonyms and alternate terminology
- Relevant disciplines and neighboring topics
- Search sources
- Search queries
- Search date
- Inclusion criteria
- Exclusion criteria

Example topic: multi-turn attacks against RAG systems.

Concept groups:

- Retrieval-augmented generation: RAG, retrieval augmented language models
- Multi-turn interaction: multi-turn, conversational, iterative, sequential
- Security: attack, adversarial, prompt injection, poisoning, jailbreak
- Agentic systems: agentic RAG, tool-using RAG, retrieval agents

Combine concept groups using appropriate Boolean operators, then adapt syntax to each database.

## 2. Paper Comparison Matrix

For every paper, extract the fields that are available:

| Field | Questions |
|---|---|
| Citation | Can the title, authors, year, and venue be verified? |
| Problem | What research problem is addressed? |
| Setting | What system, threat model, or assumptions are used? |
| Method | What attack, defense, model, or algorithm is proposed? |
| Data | What datasets, tasks, or test environments are used? |
| Evaluation | What baselines, metrics, and controls are used? |
| Findings | What results are actually reported? |
| Limitations | What limitations do the authors explicitly state? |
| Analyst notes | What additional limitations or questions can be inferred? |
| Relevance | How directly does the paper address the research question? |

Use "not reported" when information cannot be established. Do not guess.

## 3. Research Gap Taxonomy

Consider these candidate gap types:

1. Threat-model gap: an important attacker capability or assumption is not evaluated.
2. Interaction gap: a method is evaluated in isolated turns but not across longer interactions.
3. Generalization gap: results are limited to a narrow model, dataset, domain, or tool environment.
4. Evaluation gap: baselines, metrics, controls, or reproducibility are insufficient.
5. Mechanism gap: the causal explanation for an observed behavior remains unclear.
6. Defense gap: a proposed defense has untested failure modes or trade-offs.
7. Measurement gap: current metrics do not adequately measure the intended security property.
8. Conflicting-evidence gap: different studies report results that require reconciliation.

These are search prompts, not proof that a gap exists.

## 4. Evidence Levels

Classify each statement:

- Verified finding: supported by an accessible primary source.
- Reported finding: described by a paper but not independently reproduced.
- Analyst inference: reasoned from the available evidence.
- Research hypothesis: a testable proposition that has not yet been established.
- Unverified claim: insufficient evidence is currently available.

Cite the source next to the relevant claim whenever possible.

## 5. Gap Validation

Before proposing a gap:

1. Search for direct prior work.
2. Search for alternate terminology and neighboring fields.
3. Check recent surveys and related-work sections.
4. Identify the closest prior approaches.
5. Explain what remains different or unanswered.
6. State what further search could invalidate the gap claim.

Do not assert "the first" or "no prior work" without strong, documented evidence.

## 6. Experiment Planning

For each candidate direction, define:

- Research question
- Falsifiable hypothesis
- Independent variables
- Dependent variables and metrics
- Datasets and test environment
- Baselines
- Controls and ablations
- Repeated trials and uncertainty reporting
- Compute, time, and implementation costs
- Expected limitations
- Conditions that would falsify the hypothesis

Prefer controlled comparisons that isolate the effect being studied.

## 7. Prioritization

Score candidate directions from 1 to 5 on:

- Potential novelty
- Scientific significance
- Feasibility
- Evaluation clarity
- Reproducibility

Explain the basis for each score. The scores are decision aids, not objective measurements of scientific value.