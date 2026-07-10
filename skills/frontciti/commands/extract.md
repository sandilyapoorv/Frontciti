# /frontciti extract

## Purpose

Infer a design system from an existing frontend.

## Use When

Use when a product has UI patterns but lacks explicit design documentation.

## Inputs To Inspect

Pages, components, CSS, theme files, Tailwind config, screenshots, assets, icons, typography, colors, spacing, radii, shadows, and layout behavior.

## Workflow

1. Inspect the current UI and implementation.
2. Identify recurring type, color, spacing, radius, elevation, icon, and layout patterns.
3. Separate intentional patterns from accidental inconsistencies.
4. Create or update `DESIGN.md`.
5. Suggest cleanup opportunities.

## Output Expectations

The extracted system should reflect the product as it exists while identifying inconsistencies that should be resolved.

## Anti-Patterns

- Inventing a new design system instead of extracting one.
- Treating every one-off value as intentional.
- Ignoring responsive behavior.

## Acceptance Checklist

- Extracted rules match the existing product.
- Inconsistencies are identified.
- Future design decisions become easier.
