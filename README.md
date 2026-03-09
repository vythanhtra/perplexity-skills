# Perplexity Skills Library

> A curated collection of structured skill definitions for Perplexity AI — enabling repeatable, high-quality workflows across business functions.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Skills](https://img.shields.io/badge/Skills-10-blue.svg)](#skill-library)
[![Status](https://img.shields.io/badge/Status-Active-green.svg)](#)

---

## Overview

This repository contains **10 production-ready Skill definitions** for use with [Perplexity AI](https://perplexity.ai). Each skill is a structured `SKILL.md` file that documents:

- **What the skill does** — capabilities and use cases
- **What inputs it needs** — required and optional parameters
- **How to execute it** — step-by-step workflows with phases
- **What it produces** — output templates and formats
- **How to measure success** — metrics and quality benchmarks

These skills are designed for professionals, teams, and AI automation pipelines that need **consistent, repeatable research and analysis workflows** powered by Perplexity AI.

---

## Skill Library

| # | Skill | Category | Complexity | Est. Time |
|---|-------|----------|------------|----------|
| 01 | [create-skill](./create-skill/SKILL.md) | Meta / Tooling | Intermediate | 10–20 min |
| 02 | [cx-ticket-triage](./cx-ticket-triage/SKILL.md) | Customer Support | Intermediate | 5–15 min |
| 03 | [data-exploration](./data-exploration/SKILL.md) | Analytics & Research | Advanced | 15–45 min |
| 04 | [finance-audit-support](./finance-audit-support/SKILL.md) | Finance & Compliance | Advanced | 20–60 min |
| 05 | [legal-compliance](./legal-compliance/SKILL.md) | Legal & Risk | Advanced | 20–60 min |
| 06 | [legal-contract-review](./legal-contract-review/SKILL.md) | Legal & Risk | Advanced | 15–45 min |
| 07 | [marketing-competitive-analysis](./marketing-competitive-analysis/SKILL.md) | Marketing & Strategy | Advanced | 15–45 min |
| 08 | [meeting-prep](./meeting-prep/SKILL.md) | Productivity | Intermediate | 5–20 min |
| 09 | [research-summarization](./research-summarization/SKILL.md) | Knowledge Management | Intermediate | 5–30 min |
| 10 | [sales-prospecting](./sales-prospecting/SKILL.md) | Sales & Revenue | Advanced | 10–30 min |

---

## How to Use

### Option 1: Direct Reference

Open any `SKILL.md` file and follow the documented workflow step-by-step inside Perplexity AI.

```
1. Navigate to the skill folder (e.g., /meeting-prep/SKILL.md)
2. Read the Input Requirements section
3. Open Perplexity AI and follow Phase 1 → Phase 2 → Phase 3
4. Use the provided Output Template to format your results
```

### Option 2: AI Agent Integration

Each `SKILL.md` is structured to be parsed by AI agents or automation pipelines. The YAML input schemas and workflow phases are designed for programmatic consumption.

```yaml
# Example: Invoking a skill programmatically
skill: meeting-prep
inputs:
  meeting_type: sales
  participants: "Jane Smith, Acme Corp"
  meeting_objective: "Qualify for enterprise pilot"
  prep_depth: standard
```

### Option 3: Team Playbooks

Copy and adapt these skills into your team's internal playbooks, Notion wikis, or knowledge bases for standardized AI-assisted workflows.

---

## Repository Structure

```
perplexity-skills/
├── README.md                          # This file
│
├── create-skill/
│   └── SKILL.md                       # How to create new skills
│
├── cx-ticket-triage/
│   └── SKILL.md                       # Customer support triage
│
├── data-exploration/
│   └── SKILL.md                       # Data analysis workflows
│
├── finance-audit-support/
│   └── SKILL.md                       # Financial audit assistance
│
├── legal-compliance/
│   └── SKILL.md                       # Regulatory compliance research
│
├── legal-contract-review/
│   └── SKILL.md                       # Contract analysis workflows
│
├── marketing-competitive-analysis/
│   └── SKILL.md                       # Competitive intelligence
│
├── meeting-prep/
│   └── SKILL.md                       # Pre-meeting research briefs
│
├── research-summarization/
│   └── SKILL.md                       # Multi-source synthesis
│
└── sales-prospecting/
    └── SKILL.md                       # Prospect identification & outreach
```

---

## Skill File Format

Every `SKILL.md` follows a consistent schema to ensure interoperability and ease of use:

```markdown
# Skill: [Name]

## Overview          — What this skill does and why it exists
## Skill Metadata    — ID, category, complexity, time estimate, output format
## Capabilities      — 5 core capability areas with bullet descriptions
## Input Requirements — YAML schema with required and optional inputs
## Step-by-Step Workflow — Phased execution plan (Phase 1 → 2 → 3)
## Output Templates  — Copy-paste ready output structures
## Perplexity Tips   — Platform-specific optimization guidance
## Success Metrics   — How to evaluate skill performance
```

---

## Design Principles

This library is built on four core principles:

**1. Repeatability** — Every skill produces consistent, structured outputs regardless of who executes it or when.

**2. Composability** — Skills are designed to be chained. The output of `research-summarization` can feed into `meeting-prep` or `marketing-competitive-analysis`.

**3. Transparency** — Each skill documents its assumptions, limitations, and quality checks. Users always know what they're getting and where the data comes from.

**4. Human-in-the-loop** — These skills assist human judgment, not replace it. Every workflow includes checkpoints for review, validation, and critical thinking.

---

## Contributing

Contributions are welcome. To add a new skill or improve an existing one:

1. **Fork** this repository
2. **Create** a new folder: `your-skill-name/`
3. **Add** a `SKILL.md` following the [standard skill format](#skill-file-format)
4. **Reference** the [create-skill](./create-skill/SKILL.md) guide for detailed instructions
5. **Submit** a Pull Request with a clear description of what the skill does

### Contribution Standards

- Skill names must be lowercase, hyphen-separated (e.g., `market-sizing`)
- Each skill must include all required sections from the standard format
- Input schemas must use valid YAML
- Output templates must be copy-paste ready
- Success metrics must be measurable

---

## Use Cases

### For Individual Professionals
- Run competitive analysis before a sales pitch
- Prepare thoroughly for any meeting in under 20 minutes
- Summarize industry reports for executive briefings
- Review contracts for risk exposure without a lawyer on speed dial

### For Teams
- Standardize how your team uses AI for research and analysis
- Onboard new team members to AI-assisted workflows faster
- Create consistent, shareable outputs across functions
- Reduce research time by 60–75% on recurring tasks

### For AI Automation Pipelines
- Use skill definitions as structured prompts for agent orchestration
- Parse YAML input schemas for dynamic workflow invocation
- Chain skills to build multi-step research and analysis pipelines
- Extend and customize skills for domain-specific use cases

---

## License

This project is licensed under the **MIT License** — you are free to use, modify, and distribute these skills for personal and commercial purposes.

See [LICENSE](./LICENSE) for details.

---

## Acknowledgements

This library draws inspiration from the structured prompting practices of leading AI organizations and the growing community of practitioners building repeatable AI workflows.

Skill design patterns reference:
- [Anthropic's prompt engineering guidelines](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview)
- [Perplexity AI documentation](https://docs.perplexity.ai)
- Industry best practices in knowledge management and sales enablement

---

*Built with Perplexity AI. Maintained by [@vythanhtra](https://github.com/vythanhtra).*
