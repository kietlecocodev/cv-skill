# CV Reference Library Design

Date: 2026-06-08

## Goal

Add two reference folders to the `cv-skill` plugin so `cv-designer` can later use high-quality examples and ATS/recruiter screening guidance when tailoring CVs for tech roles.

The user will provide:

1. current CV or work experience, as text or PDF,
2. target job description, as text or PDF,
3. target company context, usually a company website.

This spec only covers the reference library. The full CV-generation workflow will be designed later.

## Approach

Use reconstructed templates based on real web sources.

The repository must not copy full CV templates, full resume examples, or proprietary source text unless the license clearly allows it. Instead, each reference file should:

- cite source links,
- summarize patterns,
- reconstruct original templates from cross-source patterns,
- include short examples written specifically for this skill.

## Folder 1: CV Templates

Path: `references/cv-templates/`

Target structure:

```text
references/cv-templates/
  README.md
  sources.md
  templates/
    software-engineer.md
    product-manager-tech.md
    data-ai.md
    engineering-manager.md
    founder-operator.md
  patterns/
    impact-bullets.md
    project-section.md
    skills-section.md
    seniority-signals.md
```

### Template File Contract

Each file in `templates/` should include:

- target roles,
- when to use,
- section order,
- reconstructed CV skeleton,
- bullet style,
- optimization goal,
- pitfalls,
- source links that inspired the pattern.

### Pattern File Contract

Each file in `patterns/` should include:

- pattern purpose,
- what good looks like,
- weak vs strong examples,
- role-specific notes,
- source links.

## Folder 2: ATS and Recruiter Screening

Path: `references/ats-keywords/`

Target structure:

```text
references/ats-keywords/
  README.md
  sources.md
  role-keyword-maps/
    software-engineer.md
    product-manager-tech.md
    data-ai.md
    engineering-manager.md
  best-practices/
    ats-formatting.md
    keyword-matching.md
    recruiter-screening.md
    quantified-impact.md
```

### Role Keyword Map Contract

Each file in `role-keyword-maps/` should include:

- target role family,
- core hard-skill keywords,
- systems/domain keywords,
- leadership keywords where relevant,
- tools/platform keywords,
- keyword misuse warnings,
- source links.

### Best-Practice File Contract

Each file in `best-practices/` should include:

- actionable rule,
- why it matters,
- safe examples,
- unsafe examples,
- source links.

## Source Policy

- Use real web sources.
- Store URL, title, publisher/source, accessed date, and notes in `sources.md`.
- Prefer primary or expert sources: recruiter guidance, ATS vendor guidance, hiring-manager articles, reputable career sites, and public tech resume examples.
- Use community/forum discussions only as supporting signal, not as sole authority.
- Avoid copying full examples. Reconstruct and synthesize.

## v1 Completion Criteria

The first implementation is complete when the repo contains:

- 5 reconstructed tech CV templates,
- 4 reusable CV pattern docs,
- 4 role keyword maps,
- 4 ATS/recruiter best-practice docs,
- source indexes for both reference folders,
- commit pushed to `https://github.com/kietlecocodev/cv-skill`.

## Non-Goals

- No final CV generation workflow in this phase.
- No PDF parsing implementation in this phase.
- No company website analysis workflow in this phase.
- No automated ATS scoring tool in this phase.
- No copyrighted template mirroring.

## Risks and Mitigations

- Risk: copied content or license ambiguity. Mitigation: cite sources and synthesize original templates.
- Risk: generic advice. Mitigation: role-specific files and concrete weak/strong examples.
- Risk: ATS myths. Mitigation: cite sources, phrase claims conservatively, and avoid pretending exact proprietary scoring rules are known.
- Risk: keyword stuffing. Mitigation: include misuse warnings and emphasize evidence-backed keywords only.
