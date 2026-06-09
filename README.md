# cv-skill

Claude Code plugin for designing tailored tech CVs.

## What It Does

`cv-designer` helps create a role-targeted CV from:

1. the candidate's current CV or work experience,
2. the target job description,
3. the target company website or company context.

The skill analyzes the candidate/JD/company fit, proposes CV strategy options, waits for the user to choose a direction, then produces an English designed CV as:

- design direction/spec,
- self-contained HTML/CSS CV artifact,
- Montserrat typography,
- subtle target-company brand colors,
- review notes and risk checks.

## Current Status

Working v1 skill foundation:

- core workflow,
- strategy option gate,
- designed HTML output rules,
- gentle company brand color rules,
- reconstructed tech CV references,
- ATS/recruiter keyword references,
- eval scenarios.

Still expected to improve through real CV/JD tests and tuning.

## Repository Structure

```text
skills/
  cv-designer/
    SKILL.md
    workflow.md
    intake.md
    strategy-options.md
    scoring-rubric.md
    output-formats.md
    design-output.md
    html-template-rules.md
    brand-colors.md
    evals/
      evals.json
      cases/*.md
references/
  cv-templates/
  ats-keywords/
docs/
  superpowers/
    specs/
    plans/
```

## Install on Another Device

### Option A — Install as a Claude Code plugin repo

Clone this repository into your Claude plugins directory:

```bash
git clone https://github.com/kietlecocodev/cv-skill.git ~/.claude/plugins/cv-skill
```

Then restart Claude Code or start a new session so skills are reloaded.

### Option B — Install only the skill folder

If your Claude setup only loads personal skills from `~/.claude/skills`, copy or symlink the skill folder:

```bash
git clone https://github.com/kietlecocodev/cv-skill.git ~/cv-skill
mkdir -p ~/.claude/skills
ln -s ~/cv-skill/skills/cv-designer ~/.claude/skills/cv-designer
```

If symlinks are not supported in your environment, copy instead:

```bash
cp -R ~/cv-skill/skills/cv-designer ~/.claude/skills/cv-designer
```

Restart Claude Code or start a new session after installing.

## Update on Another Device

If installed as plugin repo:

```bash
cd ~/.claude/plugins/cv-skill
git pull
```

If installed as cloned repo plus symlink:

```bash
cd ~/cv-skill
git pull
```

If installed by copying the folder, pull the repo and copy again:

```bash
cd ~/cv-skill
git pull
rm -rf ~/.claude/skills/cv-designer
cp -R ~/cv-skill/skills/cv-designer ~/.claude/skills/cv-designer
```

Restart Claude Code or open a new session after updating.

## How to Use

Ask Claude Code for CV work that matches the skill trigger, for example:

```text
Use cv-designer to tailor my CV for this job. I will provide my current CV, the JD, and the company website.
```

Recommended input:

```text
Current CV / experience:
<paste text or attach PDF>

Target JD:
<paste text or attach PDF/link>

Company:
<website URL>

Constraints:
- English CV
- HTML output
- one page or two pages
- target market/location
- anything confidential to avoid
```

Expected flow:

```text
1. Claude analyzes candidate profile, JD, and company.
2. Claude proposes 2-4 CV strategy options.
3. You choose or approve one direction.
4. Claude drafts English CV content.
5. Claude creates design spec + HTML/CSS CV.
6. Claude reviews truthfulness, JD match, ATS hygiene, recruiter scan, company fit, and design readability.
```

## Design Output Rules

Final CV output should be:

- English,
- self-contained HTML/CSS,
- Montserrat font,
- A4 printable,
- recruiter-scannable,
- fact-safe,
- subtly styled with target-company colors.

Company colors should be used gently as accents, not as dominant decoration.

## Reference Library

The plugin includes two reference libraries:

- `references/cv-templates/` — reconstructed tech CV templates and reusable writing patterns.
- `references/ats-keywords/` — role keyword maps and ATS/recruiter screening best practices.

These references synthesize public web sources. They guide CV design without copying copyrighted templates or adding unsupported claims.

## Privacy Note

This plugin may help process sensitive career information. Keep personal data, company-confidential details, compensation, and private contact information out of public examples and tests.

Do not commit real private CVs, private JDs, compensation details, addresses, phone numbers, or confidential company information into this public repository.
