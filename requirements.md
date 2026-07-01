# Requirements

## 1. Project Goal

Create a reusable ChatGPT Skill named `paper-analysis-reviewer` for deep academic paper analysis. The skill should help ChatGPT evaluate papers as a strict but fair reviewer and research training mentor.

## 2. Target Users

- Graduate students and doctoral students reading literature.
- Researchers preparing literature reviews, manuscripts, or thesis chapters.
- Teachers or supervisors training students in academic reading.
- Authors who need pre-submission critique.

## 3. Applicable Disciplines

- Management.
- Journalism and communication.
- Publishing studies.
- Humanities and social sciences.
- Empirical social science research.
- Theory, review, case, method, and interpretive papers.

## 4. Core Functions

- Classify paper type.
- Identify the paper's real research problem rather than restating the abstract.
- Analyze explicit and hidden assumptions.
- Evaluate real innovation and compare it with nearby research when information is available.
- Identify counterexamples and failure scenarios.
- Produce reviewer-style major and minor concerns.
- Suggest concrete future research directions.
- Provide specialized empirical paper checks.
- Provide specialized humanities and social science argument checks.
- Mark uncertainty and explain verification paths.

## 5. Output Format

The default output language is Chinese. Outputs should use structured headings and tables where helpful. The skill should support both short and full analysis formats through reusable templates.

## 6. Things the Skill Should Not Do

- Do not merely summarize the abstract.
- Do not invent citations, data, results, or author claims.
- Do not equate statistical significance with theoretical contribution.
- Do not turn correlation into causality without identification support.
- Do not treat questionnaire items or indicators as the theoretical concept itself.
- Do not use concept lists, slogans, or broad judgments as substitutes for analysis.

## 7. Quality Standards

- The skill directory must contain a valid `SKILL.md` with YAML frontmatter.
- The description must clearly state triggering scenarios.
- `SKILL.md` must stay concise and point to references for detailed templates.
- Reference files must contain actionable frameworks, not generic academic prose.
- The repository must contain no empty files or placeholder examples.
- The repository should be initialized with Git and include an initial commit.
- The skill should be packaged as `dist/skill.zip` when possible.

## 8. Future Extensions

- Add discipline-specific rubrics for management, communication, publishing studies, sociology, or education.
- Add a Chinese CSSCI review checklist and an English SSCI review checklist.
- Add manuscript revision templates for responding to reviewers.
- Add paper comparison templates for multi-paper literature review synthesis.
- Add thesis proposal critique workflows.
