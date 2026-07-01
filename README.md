# Literature Analysis Skill Repo

This repository contains a reusable ChatGPT Skill named `paper-analysis-reviewer`.

The skill supports deep academic paper analysis for management, journalism and communication, publishing studies, humanities, social sciences, and empirical research. It guides ChatGPT to act as a strict but fair reviewer and research mentor rather than merely summarizing abstracts.

## Directory Structure

```text
literature-analysis-skill-repo/
├── README.md
├── requirements.md
├── codex_task_prompt.md
├── paper-analysis-reviewer/
│   ├── SKILL.md
│   ├── agents/
│   │   └── openai.yaml
│   └── references/
│       ├── review_templates.md
│       ├── empirical_paper_guide.md
│       └── humanities_social_science_guide.md
└── dist/
    └── skill.zip
```

## Skill Name

`paper-analysis-reviewer`

## Suitable Use Cases

- Analyze a full paper, abstract, or pasted manuscript.
- Identify the paper's real research problem and hidden assumptions.
- Evaluate innovation, failure scenarios, reviewer concerns, and future research directions.
- Review empirical papers for concept validity, variables, models, causal identification, robustness, and overclaiming.
- Review humanities and social science papers for concept genealogy, argument chain, outline logic, paragraph progression, and language precision.

## Using `skill.zip`

The packaged file is expected at `dist/skill.zip`. Upload or import this archive into a ChatGPT/Codex Skill-compatible environment according to that environment's Skill import flow. The archive contains the `paper-analysis-reviewer/` directory with `SKILL.md`, `agents/openai.yaml`, and all reference files.

## Continuing Iteration

Update `paper-analysis-reviewer/SKILL.md` for core workflow changes. Add detailed reusable rubrics to `paper-analysis-reviewer/references/` when the guidance would make `SKILL.md` too long.

After editing, validate the skill metadata if a validation script is available, then rebuild `dist/skill.zip`.

## GitHub Version Management

Use Git to track each meaningful change. A typical GitHub setup is:

```bash
git remote add origin git@github.com:<your-user>/<your-repo>.git
git push -u origin main
```

For later updates:

```bash
git add .
git commit -m "update paper analysis reviewer skill"
git push
```
