# HTML CV Template Rules

## Purpose

Make generated HTML CVs consistent, premium, recruiter-scannable, and easy to adapt. Use these rules after content is approved and before final HTML output.

## Base Template Choice

Choose one layout based on CV strategy and company context:

| Template | Best For | Structure |
| --- | --- | --- |
| `executive-signal` | leadership, EM, senior/staff, enterprise | bold header, impact summary, metrics band, chronological body |
| `startup-operator` | founder/operator, early-stage, product/growth | narrative header, proof blocks, selected wins, flexible projects |
| `technical-credibility` | engineering, AI/ML, infra, security | compact header, skills matrix, technical experience, project proof |
| `ats-polished` | job portals, enterprise, keyword-heavy roles | single-column, minimal accent, maximum parseability |

If unsure, use `ats-polished` plus one tasteful company-color accent.

## CSS Foundation

Use these defaults unless user asks otherwise:

```css
:root {
  --primary: <company-primary>;
  --accent: <company-accent>;
  --bg: #f7f8fb;
  --paper: #ffffff;
  --text: #17202a;
  --muted: #5f6b7a;
  --line: #dfe4ea;
  --soft: color-mix(in srgb, var(--primary) 8%, white);
}

* { box-sizing: border-box; }
body {
  margin: 0;
  background: var(--bg);
  color: var(--text);
  font-family: 'Montserrat', Arial, sans-serif;
  line-height: 1.45;
}
.cv-page {
  width: 210mm;
  min-height: 297mm;
  margin: 24px auto;
  padding: 22mm 20mm;
  background: var(--paper);
  box-shadow: 0 18px 50px rgba(20, 30, 50, .10);
}
@page { size: A4; margin: 12mm; }
@media print {
  body { background: white; }
  .cv-page { margin: 0; width: auto; min-height: auto; box-shadow: none; }
}
```

## Layout Rules

- Use A4 dimensions by default.
- Keep 10-second scan path: name → target role → summary → skills → top achievements.
- Use one dominant column for experience. Use sidebars only for short metadata/skills, not core achievements.
- Put the strongest role match in the top third.
- Use company color as accent, not full-page decoration.
- Prefer subtle dividers, small chips, left border accents, or section labels.
- Keep body text readable: 10.5-12px for print, 14-16px for screen preview.
- Keep section headers distinct but not loud.
- Avoid icons unless they are decorative and text labels remain.

## Typography Rules

- Font: Montserrat only, with Arial fallback.
- Name: 28-40px, 700-800 weight.
- Target title: 12-15px, 600 weight, primary/accent color.
- Section headers: 10-12px, uppercase, letter-spaced, 700 weight.
- Body: 10.5-12px print, 400-500 weight.
- Bullets: concise, 1-2 lines where possible.

## Color Rules

- Primary brand color can be used for name accent, section rules, tags, or metric labels.
- Accent color should appear sparingly.
- Text must stay dark on light background unless contrast is clearly high.
- Never place long body text on saturated color blocks.
- If company palette is loud, mute it for CV use.

## Required HTML Sections

Use semantic sections:

```html
<header class="cv-header">...</header>
<section class="summary">...</section>
<section class="skills">...</section>
<section class="experience">...</section>
<section class="projects">...</section>
<section class="education">...</section>
```

Omit empty sections. Do not invent content to fill layout.

## Anti-Slop Rules

Avoid:

- generic gradient hero blocks,
- skill progress bars,
- random emojis/icons,
- oversized decorative sidebars,
- low-contrast pastel text,
- dense cards inside cards,
- fake metrics used as visual highlights,
- two-column layouts that break chronological reading,
- colors unrelated to the target company.

## Quality Bar

A good HTML CV should feel like a premium one-page product brief: restrained, aligned, high contrast, sharp hierarchy, and easy to print.
