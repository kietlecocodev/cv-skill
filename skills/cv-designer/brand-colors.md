# Gentle Brand Color Usage

## Purpose

Use target company colors to make the CV feel tailored, but keep the design professional, subtle, readable, and CV-first. Brand colors are seasoning, not the main dish.

## Extraction Order

When company context is available, identify colors in this order:

1. Company logo primary color.
2. Website primary CTA/link color.
3. Website accent color.
4. Neutral/background color.
5. Text color.

If exact colors cannot be inspected, infer a conservative palette and label it:

```markdown
Brand palette inferred from visible company website/logo. Confirm exact brand colors before production use.
```

## Usage Budget

Default brand color usage should be gentle:

- Primary color: 5-10% of visible page area.
- Accent color: 1-3% of visible page area.
- Neutral/background: 85-94% of page area.
- Body text: dark neutral, never brand color for long paragraphs.

## Safe Uses

Use brand color for:

- thin section dividers,
- small labels or chips,
- target role subtitle,
- metric labels,
- left border accents,
- small header rule,
- link/contact highlights.

## Avoid

Do not use brand color for:

- full-page saturated backgrounds,
- long body text,
- large sidebars unless extremely muted,
- decorative gradients,
- skill bars,
- huge blocks behind experience bullets,
- low-contrast text,
- multiple competing accent colors.

## Palette Rules

- Use one primary brand color and one optional accent.
- If company colors are loud, create a muted tint for backgrounds.
- Keep text contrast high.
- Use neutral paper/background and dark text.
- Do not invent colorful palettes unrelated to the company.

## Example

For a company with dark navy and electric blue:

```css
:root {
  --primary: #0b1f3a;
  --accent: #2f7df6;
  --bg: #f6f8fb;
  --paper: #ffffff;
  --text: #17202a;
  --muted: #667085;
  --line: #d8e0ea;
  --soft: #eef5ff;
}
```

Use navy for headings or rules, blue for small highlights, and white/neutral for most surfaces.

## Review Question

Before finalizing, ask internally: “If the logo colors were removed, would this still be a strong CV?” If no, simplify the design.
