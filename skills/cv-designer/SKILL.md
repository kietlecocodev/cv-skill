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

## Required Behavior

1. Collect candidate CV/experience, target JD, and company context.
2. If critical context is missing, ask before drafting or label assumptions if user wants to proceed.
3. Analyze candidate profile, JD, and company before writing CV text.
4. Present 2-4 CV strategy options before drafting.
5. Wait for user to choose or approve a CV direction.
6. Draft only from real candidate evidence.
7. Produce final output in English as a design spec plus self-contained HTML/CSS CV artifact.
8. Review with truthfulness, JD match, ATS hygiene, recruiter scan, company-fit, and design-readability checks.

## Supporting Guides

Load these when doing the corresponding work:

- `workflow.md` — end-to-end process and hard gate.
- `intake.md` — input requirements and extraction checklists.
- `strategy-options.md` — CV type options and recommendation format.
- `scoring-rubric.md` — final review checklist and scores.
- `output-formats.md` — strategy, HTML CV, and final delivery formats.
- `design-output.md` — English HTML/CSS artifact rules, Montserrat typography, and company brand color usage.
- `brand-colors.md` — gentle company color extraction and subtle usage rules.
- `html-template-rules.md` — premium layout system, CSS defaults, print rules, and anti-slop design constraints.

## Reference Library

Consult these references when relevant:

- `references/cv-templates/` for reconstructed role-family templates and CV section patterns.
- `references/ats-keywords/` for role keyword maps and ATS/recruiter screening best practices.

References guide structure and wording only. The final CV must be based on the candidate's real experience, the target JD, and verified company context.

## Non-Negotiable Rules

- No final CV draft before CV strategy options and user approval.
- Never invent metrics, employers, tools, education, certifications, or scope.
- Mark missing or uncertain facts instead of filling them silently.
- Prefer exact JD terminology only when it truthfully matches candidate experience.
- Preserve interview defensibility: every strong claim should be explainable by the candidate.
- Do not leak sensitive/confidential details unnecessarily.
- Final CV must be written in English.
- Final artifact must include design spec plus self-contained HTML/CSS.
- Use Montserrat as default font.
- Use target company brand colors gently when available; label inferred colors when exact values are unknown.
- Brand colors should be accents, not dominant page decoration.

## Baseline Risks Prevented

Without this skill, agents may draft too early, skip company/JD positioning, choose one generic CV style, overfit keywords, create weak bullets, or add claims hard to defend in interviews.
