<h1 align="center">Awesome Legal Skills</h1>

<p align="center">
  <strong>AI Agent Skills for Legal Professionals</strong>
</p>

<p align="center">
  <a href="https://lawvable.com/skills">
    <img src="https://img.shields.io/badge/Skills-9%20Available-4F46E5?style=flat-square" alt="Skills Available" />
  </a>
  <a href="https://github.com/lawvable/awesome-legal-skills/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg?style=flat-square" alt="License" />
  </a>
  <a href="https://makeapullrequest.com">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome" />
  </a>
</p>

<p align="center">
  <a href="https://lawvable.com/en/skills">Browse</a> &bull;
  <a href="https://lawvable.com/en/learn">Learn</a> &bull;
  <a href="#getting-started">Get Started</a> &bull;
  <a href="#contributing">Contribute</a>
</p>

## What are Agent Skills?

Agent Skills are portable instructions that teach AI agents how to perform specific tasks your way. Each skill is a self-contained package of prompts, templates, and guidelines that agents load on-demand to handle specialized workflows.

For legal professionals, this means encoding your expertise into reusable AI workflows. Draft GDPR-compliant privacy policies. Review NDAs using your firm's methodology. Create due diligence checklists that match your standards.

**Write once, use everywhere** — Skills are an emerging standard for AI agents. Currently supported by Claude, with adoption growing across the industry.

### What a Skill Looks Like

```yaml
---
name: nda-reviewer
description: Reviews NDAs to identify one-sided terms, missing protections, and negotiation points
---

# NDA Reviewer

Analyzes Non-Disclosure Agreements for legal risks and negotiation opportunities.

## When to Activate

Activates when reviewing mutual or one-way NDAs before signing or negotiating terms.

## Practical Guidance

1. Identify the disclosing and receiving parties
2. Check the definition of "Confidential Information"
3. Verify the term and survival period
4. Review permitted disclosures
5. Flag one-sided obligations in mutual NDAs

## Guidelines

- Flag missing carve-outs for publicly available information
- Flag unlimited duration for obligations
- Flag missing return/destruction clauses
- Flag injunctive relief without proving damages
```

### How Skills Work

Skills use a progressive loading architecture for efficiency:

1. **Discovery** (~100 tokens): Agent scans skill metadata to find relevant matches
2. **Activation** (<5k tokens): Full instructions load when Agent determines the skill applies
3. **Resources**: Templates, scripts, and reference files load only as needed

This design allows multiple skills to remain available without consuming your agent's context window.

## Available Skills

### Commercial Law

| Skill | Author | Description |
|-------|--------|-------------|
| **[nda-review-en](./skills/nda-review-en-jamie-tso)** | [Jamie Tso](https://github.com/jamietso/nda-review-skill) | Review incoming unilateral commercial NDAs |

### Corporate Law

| Skill | Author | Description |
|-------|--------|-------------|
| **[whistleblower-policy-fr](./skills/whistleblower-policy-fr-malik-taiar)** | [Malik Taiar](https://www.linkedin.com/in/malik-taiar/) | Assess or draft compliant whistleblower policies under EU Directive and Sapin II law | 

### Privacy Law

| Skill | Author | Description |
|-------|--------|-------------|
| **[privacy-policy-fr](./skills/privacy-policy-fr-malik-taiar)** | [Malik Taiar](https://www.linkedin.com/in/malik-taiar/) | Draft GDPR-compliant privacy policies following CNIL recommendations |
| **[cookie-policy-fr](./skills/cookie-policy-fr-malik-taiar)** | [Malik Taiar](https://www.linkedin.com/in/malik-taiar/) | Create cookie policies compliant with GDPR and ePrivacy directive |

### Document Processing

| Skill | Author | Description |
|-------|--------|-------------|
| **[docx](./skills/docx-processing-en-anthropic)** |  [Anthropic](https://github.com/anthropics/skills) | Create, edit, and analyze Word documents with tracked changes, comments, and formatting preservation |
| **[pdf](./skills/pdf-processing-en-anthropic)** | [Anthropic](https://github.com/anthropics/skills) | Extract text and tables, create new PDFs, merge/split documents, and handle form fields |
| **[xlsx](./skills/xlsx-processing-en-anthropic)** | [Anthropic](https://github.com/anthropics/skills) | Work with spreadsheets including formulas, formatting, data analysis, and visualization |
| **[pptx](./skills/pptx-processing-en-anthropic)** | [Anthropic](https://github.com/anthropics/skills) | Build and modify presentations with layouts, templates, charts, and speaker notes |

### Utility

Tools for building and extending skills.

| Skill | Author | Description |
|-------|--------|-------------|
| **[skill-creator](./skills/skill-creator-en-anthropic)** | [Anthropic](https://github.com/anthropics/skills) | Interactive guide for creating new skills with structured Q&A |

## Getting Started

1. Download a skill folder from this repository
2. Go to **[claude.ai/settings/capabilities](https://claude.ai/settings/capabilities)** and enable the **Code execution and file creation** toggle
3. Scroll to the **Skills** section and click the **Add** button
4. Upload your downloaded Skill — Claude activates automatically when relevant

> Skills require a Claude Pro, Max, Team, or Enterprise plan.

## Security

Skills can include executable scripts. Only install from trusted sources, review code before use, and never include client data. Ensure skills align with your firm's confidentiality policies and professional responsibility obligations.

## Contributing

We welcome contributions. See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

## License

This repository is licensed under the [Apache License 2.0](./LICENSE). Individual skills may have specific licensing terms (check each skill's folder for details).

## Acknowledgments

Special thanks to the Anthropic team for developing the Skills feature and publishing detailed examples.
