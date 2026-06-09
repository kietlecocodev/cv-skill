# cv-skill

Claude Code plugin for CV design workflows.

## Current status

v0 scaffold only. The first skill, `cv-designer`, captures the basic intent: design a tailored CV from the user's experience, a target job description, and company context.

Detailed workflow, CV templates, ATS guidance, examples, and evaluation scenarios will be designed later.

## Structure

```text
skills/
  cv-designer/
    SKILL.md
```

## Reference Library

The plugin includes two reference libraries:

- `references/cv-templates/` — reconstructed tech CV templates and reusable writing patterns.
- `references/ats-keywords/` — role keyword maps and ATS/recruiter screening best practices.

These references synthesize public web sources. They should guide CV design without copying copyrighted templates or adding unsupported claims.

## Privacy note

This plugin may help process sensitive career information. Keep personal data, company-confidential details, compensation, and private contact information out of public examples and tests.
