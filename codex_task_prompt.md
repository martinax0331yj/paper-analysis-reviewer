# Reusable Codex Task Prompt

Use this prompt when asking Codex to maintain or extend this Skill:

```text
Please update the local ChatGPT Skill repository at `literature-analysis-skill-repo/`.

The Skill is named `paper-analysis-reviewer` and is used for deep academic paper analysis in management, journalism and communication, publishing studies, humanities, social sciences, and empirical research.

Follow ChatGPT Skill conventions:

1. Keep `paper-analysis-reviewer/SKILL.md` valid with YAML frontmatter containing only `name` and `description`.
2. Keep `SKILL.md` concise and operational.
3. Put detailed reusable rubrics, templates, and checklists in `paper-analysis-reviewer/references/`.
4. Ensure `SKILL.md` explicitly points to any reference file that should be loaded for a task.
5. Keep the default output language Chinese unless the user asks otherwise.
6. Require uncertainty labels and verification paths when information is incomplete.
7. Do not create unrelated scripts, large assets, empty files, or placeholder examples.
8. Validate the Skill if a validation script is available.
9. Rebuild `dist/skill.zip` after changes.
10. Commit the changes to Git with a clear commit message.

When adding new features, preserve the skill's core stance: strict but fair academic reviewer plus research training mentor. The skill should analyze real problem consciousness, hidden assumptions, actual innovation, failure scenarios, reviewer concerns, future research directions, empirical method logic, concept genealogy, outline logic, and writing logic. It must not merely summarize abstracts.
```
