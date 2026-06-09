---
name: cv-designer
description: Use when tailoring or designing a CV/resume for a specific job application using the candidate's experience, target job description, company context, seniority level, or application goal.
---

# CV Designer

## Overview

Designs tailored tech CVs from the candidate's real experience, the target JD, and company context. Core principle: analyze first, offer CV strategy options, get user direction, then draft without inventing facts.

## When to Use

Use for:

- tailoring a CV/resume to a specific job description,
- mapping career experience to role requirements,
- adapting CV tone for a target company,
- choosing which CV positioning/version best fits a target application,
- deciding what to emphasize, remove, or rewrite for an application.

Do not use for:

- fabricating experience, credentials, metrics, or employment history,
- exposing sensitive personal data in public examples,
- writing generic CV advice with no target role or context,
- drafting a final CV before the user chooses or approves a CV direction.

## Required Input

Accept any mix of:

1. Candidate CV or experience history as text/PDF.
2. Target JD as text/PDF/link.
3. Target company website or company context.

If a critical input is missing, ask for it before drafting. If the user wants to proceed with partial context, clearly label assumptions and risks.

## Core Workflow

1. **Intake** — collect candidate experience, JD, company context, target role, seniority, market/location, and constraints.
2. **Candidate Profile Extraction** — extract roles, achievements, metrics, skills, projects, education, constraints, and sensitive/uncertain claims.
3. **JD Analysis** — identify must-haves, nice-to-haves, responsibilities, keywords, seniority signals, and hidden priorities.
4. **Company Analysis** — infer company stage, product/business model, culture/tone, likely hiring signals, and CV tone implications.
5. **Match Strategy** — map strongest overlaps, gaps, transferable evidence, and claims to avoid.
6. **CV Strategy Options** — propose 2-4 CV directions the user can choose from.
7. **User Direction Gate** — do not draft final CV until user selects or approves a direction.
8. **Draft CV** — write selected version using real evidence, target keywords, and reference library patterns.
9. **Review** — run truthfulness, ATS, recruiter scan, keyword, and readability checks.
10. **Final Output** — provide final CV plus change notes, missing info, and interview risk notes.

## CV Strategy Options Gate

After analyzing the JD and company, always present CV strategy options before drafting.

Each option must include:

- CV type name,
- why it fits this JD/company,
- what it emphasizes,
- what it downplays,
- risk/tradeoff,
- recommended use case.

Common option types:

| CV Type | Best For | Emphasizes | Downplays |
| --- | --- | --- | --- |
| ATS-first CV | job portals, enterprise, keyword-heavy JDs | exact JD match, standard structure, parseability | distinctive narrative/design |
| Impact-led tech CV | startups/scaleups, product/engineering/data roles | shipped work, metrics, ownership, business/product impact | broad career story |
| Founder-operator CV | early-stage startups, operator/product/growth roles | zero-to-one, ambiguity, customer/growth/revenue ownership | formal enterprise process |
| Specialist credibility CV | AI/ML/infra/security/backend specialist roles | technical depth, systems/projects, domain proof | generalist positioning |
| Leadership/seniority CV | EM, lead, staff, head roles | team scope, strategy, mentoring, delivery, cross-functional influence | hands-on implementation detail unless needed |

Example format:

```markdown
## Recommended CV Directions

### Option A — ATS-first Product CV
Best if applying through a job portal.
Emphasizes: JD keyword match, product metrics, roadmap ownership.
Downplays: founder narrative.
Risk: less memorable to founder/team readers.

### Option B — Founder-Operator Product CV
Best if the company is early-stage and the role values ambiguity.
Emphasizes: zero-to-one ownership, growth, customer discovery.
Downplays: formal enterprise PM process.
Risk: weaker for ATS if not keyword-balanced.

### Recommendation
Use Option B as the main version, with ATS keyword hygiene from Option A.
```

## Drafting Rules

- Never invent metrics, employers, tools, education, certifications, or scope.
- Mark missing or uncertain facts instead of filling them silently.
- Prefer exact JD terminology only when it truthfully matches candidate experience.
- Use metrics when real; otherwise use observable outcomes.
- Keep ATS readability unless the user explicitly chooses a design-forward version.
- Preserve interview defensibility: every strong claim should be explainable by the candidate.

## Reference Library

When tailoring a tech CV, consult these references when relevant:

- `references/cv-templates/` for reconstructed role-family templates and CV section patterns.
- `references/ats-keywords/` for role keyword maps and ATS/recruiter screening best practices.

Use references as guidance only. The final CV must be based on the candidate's real experience, the target JD, and verified company context.

## Review Checklist

Before finalizing, check:

- CV direction chosen or approved by user.
- Must-have JD requirements are addressed where truthfully supported.
- Important keywords appear in skills and experience context, not stuffed.
- Most relevant achievements appear in the top third.
- Claims with missing evidence are flagged.
- Formatting is ATS-readable unless user chose otherwise.
- Tone matches company context and seniority.
- CV does not leak sensitive/confidential details unnecessarily.

## Baseline Risks Found

Without this skill, agents may:

- draft too early from vague inputs,
- skip company/JD positioning analysis,
- choose one generic CV style without offering alternatives,
- overfit to JD keywords,
- create weak bullets without verified metrics,
- add claims that are hard to defend in interviews.

This skill prevents those failures by requiring analysis, CV direction options, user approval, and fact-safe drafting.

## Current Status

Core workflow v1 is defined. Remaining work: supporting files, example outputs, eval scenarios, and real-data tuning.
