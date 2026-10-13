# Paper Research

A reusable Agent Skill for academic literature reviews, research gap analysis, paper comparison, and research planning.

## Overview

**Paper Research** is a reusable skill designed to help AI agents conduct structured, evidence-based academic research.

It provides a repeatable workflow for understanding a research topic, organizing related papers, identifying potential research gaps, and turning promising ideas into testable research questions.

The skill follows the [Agent Skills specification](https://agentskills.io/specification) and is designed for compatible agent platforms.

## Features

- **Literature Review** — Define research questions, organize relevant literature, and summarize research themes.
- **Paper Comparison** — Compare research problems, methods, datasets, evaluation settings, findings, and limitations.
- **Research Gap Analysis** — Identify potential gaps and distinguish evidence-backed findings from hypotheses.
- **Research Planning** — Develop research questions, experimental designs, baselines, metrics, and ablation studies.
- **Evidence-Based Reporting** — Use a consistent report structure and explicitly document uncertainty.
- **Research Integrity** — Avoid fabricated citations, unsupported novelty claims, and unverified experimental results.

## Project Structure

```text
paper-research/
├── SKILL.md
├── references/
│   └── research-method.md
├── assets/
│   └── report-template.md
├── tests/
│   └── test-cases.md
└── README.md
```

| File | Description |
|---|---|
| `SKILL.md` | Skill metadata, instructions, workflow, and usage guidance |
| `references/research-method.md` | Literature comparison, research gap taxonomy, and experiment planning methods |
| `assets/report-template.md` | Reusable research report template |
| `tests/test-cases.md` | Manual test cases for evaluating expected behavior |
| `README.md` | Project overview and usage instructions |

## Installation

### Option 1: Clone from GitHub

Replace `YOUR_USERNAME` with your GitHub username.

```bash
git clone https://github.com/YOUR_USERNAME/paper-research.git
cd paper-research
```

### Option 2: Install into a Compatible Agent

This project follows the Agent Skills directory format.

To use it, place the complete `paper-research` directory in a Skills discovery directory supported by your agent.

The exact installation path depends on the host platform. Consult your agent's documentation for its supported Skills directory and loading behavior.

Keep the entire directory structure intact so that the agent can access the reference guide and report template.

## Usage

Once the skill is installed and recognized by a compatible agent, try the following prompts.

### Example 1: Literature Review

```text
Review the literature on multi-turn attacks against RAG systems.

Identify relevant research themes, compare existing approaches,
and summarize the current state of the field.
```

### Example 2: Research Gap Analysis

```text
Analyze potential research gaps in trajectory-aware attacks
against agentic RAG systems.

Compare related work, examine alternative terminology,
and distinguish evidence-backed gaps from hypotheses.
```

### Example 3: Paper Comparison

```text
Compare these five papers in terms of research objectives,
methods, datasets, evaluation metrics, findings, and limitations.
```

### Example 4: Experimental Design

```text
Based on the identified research gaps, propose an experimental plan.

Include research questions, hypotheses, baselines, datasets,
evaluation metrics, controls, ablation studies, and limitations.
```

## Research Workflow

The skill follows a structured research process:

1. Define the research question and scope.
2. Identify keywords, synonyms, and related terminology.
3. Plan and conduct literature searches using available tools.
4. Verify paper metadata and source evidence.
5. Compare existing research methods and findings.
6. Identify and validate candidate research gaps.
7. Prioritize potential research directions.
8. Design experiments to test the proposed hypotheses.
9. Produce a structured research report.
10. Review citations, uncertainty, and limitations.

## Important Limitations

- The skill does not independently provide web search, academic database access, or full-text access.
- Live literature searches require compatible search tools or other accessible research sources.
- Findings based only on abstracts must be labeled accordingly.
- A missing search result does not prove that a research idea is novel.
- Citations, publication details, and research claims should be verified against reliable sources.
- Research gap suggestions are hypotheses until sufficiently validated against prior work.

## Testing

Review the manual test cases in `tests/test-cases.md`.

Basic checks should verify that:

- The skill metadata is valid.
- Required files are present.
- Referenced resources are accessible.
- The agent follows the research workflow.
- Unsupported citations and novelty claims are not presented as established facts.

Static checks alone do not guarantee correct behavior. Test the skill inside the intended host agent as well.

## Contributing

Suggestions, issue reports, and improvements are welcome.

When proposing changes, please prioritize:

- Clear and reusable research instructions.
- Reliable citation and evidence handling.
- Reproducible research workflows.
- Useful test cases.
- Compatibility with the Agent Skills specification.

## License

No license has been selected yet.

Before redistributing this project, add a `LICENSE` file specifying the terms under which others may use, modify, and redistribute it.

## Disclaimer

This skill assists with research organization and analysis. It does not guarantee literature coverage, research novelty, or the correctness of every generated conclusion. Important findings should be independently verified.