# Contributing

Thank you for your interest in contributing to Lawvable Skills.

## Before You Start

- Ensure your skill is based on a **real use case**, not a hypothetical scenario
- Search existing skills to avoid duplicates
- Verify your skill works on at least one platform (Claude.ai, Claude Code, etc.)
- If inspired by someone's workflow, prepare to give attribution

## Skill Structure

Create a folder with your skill name (lowercase, hyphens only):

```
skill-name/
├── SKILL.md          # Required: instructions with YAML frontmatter
├── scripts/          # Optional: helper scripts
├── templates/        # Optional: document templates
└── resources/        # Optional: reference materials
```

## SKILL.md Template

Copy [`template/SKILL.md`](./template/SKILL.md) and fill in all sections. Keep under 500 lines.

## Legal Guidelines

- **Jurisdictions**: State geographic scope and regulatory frameworks (GDPR, CCPA, etc.)
- **Accuracy**: Reference authoritative sources with version dates
- **Confidentiality**: Never include real client data; use fictional examples
- **Attribution**: Credit sources with `**Inspired by:** [Source]`

## Submit a Skill

1. Fork the repository
2. Create branch: `git checkout -b add-skill-name`
3. Add your skill to `skills/your-skill-name/`
4. Update `README.md` with your skill (alphabetical order)
5. Submit PR with title: `Add [Skill Name] skill`

### Checklist

- [ ] Solves a real legal workflow problem
- [ ] SKILL.md has valid frontmatter (`name` and `description`)
- [ ] Skill name is lowercase with hyphens only
- [ ] Examples show practical usage
- [ ] Jurisdictions documented (if applicable)
- [ ] No client data or confidential information
- [ ] Tested on at least one platform
- [ ] Works across agent platforms (Claude, Cursor, etc.)

To update an existing skill, fork, make changes, test, and submit a PR explaining what changed.

## Ideas for Skills

Need inspiration? Areas where skills would be valuable:

- Contract clause libraries
- Due diligence checklists
- Legal document templates
- Compliance frameworks (SOC 2, ISO 27001)
- Research methodologies
- Court filing procedures
- Client intake workflows

## Questions?

Open an [issue](https://github.com/lawvable/agent-skills/issues) for help. Be respectful and credit original sources.
