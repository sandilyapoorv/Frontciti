# Typography

Typography carries hierarchy and personality.

## Register Rules

Brand surfaces:

- Choose type from the brief's physical world and voice.
- Use fluid display scales where appropriate.
- Pair fonts only when contrast is meaningful.
- Avoid reflex choices and currently saturated AI defaults.

Product surfaces:

- One well-tuned sans family is often best.
- Use fixed `rem` scales rather than fluid display type.
- Use tighter ratios because product UIs contain many roles.
- Use tabular figures for data.

## Scale

Most interfaces need roles, not many arbitrary sizes:

- Caption.
- Secondary.
- Body.
- Subheading.
- Heading.
- Display.

Use strong enough contrast that headings, body, metadata, and actions are recognizable at a glance.

## Readability

- Body text should usually be at least 16px.
- Keep prose measure around 45-75 characters.
- Use `text-wrap: balance` for headings and `text-wrap: pretty` for prose where supported.
- Avoid clipped descenders in italic display text.
- Light text on dark backgrounds often needs more line-height and sometimes slightly heavier weight.

## Font Loading

- Prefer project conventions: `next/font`, local fonts, or existing font utilities.
- Use `font-display: swap` or an established metric fallback strategy.
- Load only needed weights.
- Do not link random external fonts when the app already has a font pipeline.

## Avoid

- Too many font families.
- Similar-but-not-identical font pairings.
- Decorative fonts for body text.
- Body text below readable size.
- Over-tight display tracking.
- Text overflow at mobile or tablet widths.
