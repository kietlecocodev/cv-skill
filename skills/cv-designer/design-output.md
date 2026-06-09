# Designed HTML CV Output

## Purpose

Produce the final CV as an English, design-first HTML/CSS artifact plus a short design spec. The design should adapt to the target company while preserving recruiter readability and interview-safe content.

## Non-Negotiables

- Final CV language: English.
- Final designed artifact: HTML/CSS.
- Font: Montserrat.
- Color palette: use target company brand colors when available.
- If brand colors are unavailable, infer a conservative palette from the company website/logo and label it as inferred.
- Do not use colors or layout choices that reduce readability.
- Do not sacrifice truthfulness or ATS/recruiter clarity for decoration.

## Brand Color Extraction

When company website/context is available, identify:

- primary brand color,
- secondary/accent color,
- neutral/background color,
- text color,
- brand tone: enterprise, playful, technical, luxury, minimalist, developer-first, AI-native, fintech-trust, consumer-growth.

If exact colors cannot be inspected, state assumptions:

```markdown
Brand colors inferred from visible company website/logo. Confirm before production use.
```

## Design Spec Output

Before or alongside HTML, include:

```markdown
## CV Design Direction

### Brand Inspiration
- Company colors:
- Supporting neutrals:
- Visual tone:
- Why it fits the company:

### Typography
- Font: Montserrat
- Name:
- Section headers:
- Body:
- Metadata:

### Layout
- Format:
- Header style:
- Section grid:
- Sidebar/no-sidebar:
- Spacing:
- ATS-safe notes:

### Color Usage
- Primary:
- Accent:
- Background:
- Text:
- Dividers:
```

## HTML Artifact Requirements

HTML/CSS should be self-contained unless user asks otherwise.

Required structure:

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
    <!-- CV content -->
  </main>
</body>
</html>
```

## Layout Defaults

- Single-page or two-page depending on candidate seniority and user constraint.
- Clean header with name, target positioning, location/contact links.
- Strong top third: summary, core skills, strongest evidence.
- Use subtle brand accents: lines, section labels, small blocks, not heavy backgrounds.
- Avoid skill bars, decorative icons that replace text, dense multi-column body content, and low contrast.

## ATS Note

Designed HTML is best for direct sharing, recruiter email, portfolio, or manual review. If the user applies through a job portal, also provide an ATS-safe Markdown/text version or explain how to simplify the HTML content.
