# dev-skills

skills for software engineering

Repository documentation is written in English. Skill content (`SKILL.md` and everything under it) stays in the language the skill targets — Chinese for `code-review-format`, since its rules define Chinese review report output.

## Repository Layout

Each skill lives in its own directory under `skills/`:

```
skills/
└── <skill-name>/
    ├── SKILL.md       # Required: YAML frontmatter (name / description) + instructions
    ├── assets/        # Optional: templates, samples, and other files shipped with the skill
    ├── references/    # Optional: supplementary reference docs
    └── scripts/       # Optional: helper scripts
```

`skills/` is a default discovery directory for `npx skills`. To add a new skill, create a directory named after it under `skills/` and drop in a `SKILL.md` — no registration needed.

## Available Skills

| Skill                                                    | Description                                                                                                                                        |
| -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| [code-review-format](skills/code-review-format/SKILL.md) | Output specification for code review and re-review: scope, dimensions, severity, numbering, evidence, structure, re-review, style, and self-checks |

## Installation

```bash
# List the skills available in this repository
npx skills add gzliudan/dev-skills --list

# Pick skills to install interactively
npx skills add gzliudan/dev-skills

# Install a specific skill (project scope by default)
npx skills add gzliudan/dev-skills --skill code-review-format

# Install to the user-level (global) directory
npx skills add gzliudan/dev-skills --skill code-review-format -g
```
