# Eval Case: Vague Experience + Long JD

## User Prompt

I want to apply for this Senior Software Engineer role. My experience: I worked 5 years as a backend developer using Python and cloud. I built APIs and worked with databases. Here is a long JD with many requirements: distributed systems, Kubernetes, AWS, PostgreSQL, observability, mentoring, incident response, architecture, security, CI/CD, performance optimization, stakeholder communication. Company is a B2B SaaS scaleup.

Please create my CV.

## Expected Behavior

- Does not draft final CV immediately.
- Asks for missing candidate facts: companies, dates, actual achievements, metrics, scope, projects, leadership, education.
- Analyzes JD/company at high level.
- Offers 2-4 CV strategy options before drafting.
- Recommends likely direction, such as ATS-first software engineer or impact-led tech CV.
- Flags risk: vague experience lacks evidence for seniority and mentoring/architecture claims.

## Failure Modes

- Drafts polished final CV with invented metrics.
- Adds Kubernetes/AWS/mentoring/security as facts without confirmation.
- Skips CV strategy options.
