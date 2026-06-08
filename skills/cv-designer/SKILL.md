---
name: cv-designer
description: Use when tailoring or designing a CV/resume for a specific job application using the candidate's experience, target job description, company context, seniority level, or application goal.
---

# CV Designer

## Overview

Helps design a tailored CV from the candidate's real experience, the target JD, and company context. v0 scaffold: collect context first, avoid inventing facts, and prepare for deeper skill design later.

## When to Use

Use for:

- tailoring a CV/resume to a specific job description,
- mapping career experience to role requirements,
- adapting CV tone for a target company,
- deciding what to emphasize, remove, or rewrite for an application.

Do not use for:

- fabricating experience, credentials, metrics, or employment history,
- exposing sensitive personal data in public examples,
- writing generic CV advice with no target role or context.

## v0 Working Pattern

1. Collect candidate context: roles, years, achievements, metrics, skills, projects, education, constraints.
2. Collect target context: JD, company information, role seniority, location/market, application goal.
3. Identify missing high-impact facts before drafting.
4. Map real evidence to JD requirements.
5. Propose CV structure and emphasis before producing final text.
6. Mark uncertain claims for user confirmation.

## Baseline Risk Found

Without a dedicated skill, an agent may draft too early from vague inputs, overfit to JD keywords, or create weak bullets without verified metrics. This skill should force context collection and fact safety before CV generation.

## Current Status

Detailed CV workflow, ATS rules, templates, examples, quality rubric, and evaluation scenarios are pending deeper design with the user.
