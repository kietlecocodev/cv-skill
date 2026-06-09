# Output Formats

## Strategy Options Output

Use before drafting:

```markdown
## Recommended CV Directions

### Option A — <CV Type>
Best if: <condition>
Why it fits: <JD/company reason>
Emphasizes: <strengths>
Downplays: <less relevant story>
Risk: <tradeoff>

### Recommendation
<recommended option and why>

Please choose one option, or approve the recommendation.
```

## Draft Content Output

All final CV content must be written in English. Draft content can be shown before HTML generation when useful:

```markdown
# <Candidate Name>
<Location> · <Email> · <Phone> · <LinkedIn> · <Portfolio/GitHub>

## Summary
<2-4 lines tailored to role>

## Skills
- <group>: <skills>

## Experience
### <Title> — <Company>
<Date range>
- <impact bullet>

## Projects
### <Project>
- <impact bullet>

## Education
<education/certification>
```

## Designed Final Output

Default final output is a design spec plus self-contained HTML/CSS CV artifact.

```markdown
## CV Design Direction

### Brand Inspiration
- Company colors:
- Supporting neutrals:
- Visual tone:
- Why it fits the company:

### Typography
- Font: Montserrat
- Hierarchy:

### Layout
- Format:
- Header style:
- Section grid:
- ATS-safe notes:

## HTML CV

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Candidate CV</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: <company-primary>;
      --accent: <company-accent>;
      --bg: <background>;
      --text: <text>;
      --muted: <muted>;
      --line: <divider>;
    }
    body { font-family: 'Montserrat', Arial, sans-serif; }
  </style>
</head>
<body>
  <main class="cv-page">
    <!-- English CV content -->
  </main>
</body>
</html>
```
```

## Final Delivery Output

After draft and design review, include:

```markdown
## Final CV Design Spec
<design direction>

## Final HTML CV
<html artifact>

## What Changed
- <major positioning, content, and design changes>

## Missing Info / User Confirmation Needed
- <facts that need confirmation>

## Interview Risk Notes
- <claims user should be ready to defend>

## ATS-Safe Notes
- <how to adapt for job portals if needed>

## Review Scores
- Truthfulness: <1-5>
- JD Match: <1-5>
- ATS Hygiene: <1-5>
- Recruiter Scan: <1-5>
- Company Fit: <1-5>
- Design Readability: <1-5>
```

## Variant Rule

If user asks for multiple versions, produce separate sections:

- Designed HTML version,
- ATS-safe Markdown/text version,
- short recruiter message or cover note if requested.
