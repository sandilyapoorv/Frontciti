# /frontciti init

## Purpose

Create or update persistent product and design context for future frontend work.

## Use When

Use when a project lacks clear design direction, product context, or reusable UI rules.

## Inputs To Inspect

README files, package files, routes, app structure, components, styles, assets, screenshots, existing copy, and any product documentation.

## Workflow

1. Infer product type, audience, core workflows, conversion goals, current UX, visual tone, and stack.
2. Create `PRODUCT.md` and `DESIGN.md` from the templates when missing.
3. Update existing files without deleting useful context.
4. Mark unknowns as assumptions or open questions.

## Output Expectations

`PRODUCT.md` should cover users, jobs, workflows, business goals, references, anti-references, stage, constraints, and unknowns.

`DESIGN.md` should cover personality, typography, color, layout, components, motion, accessibility, density, responsive rules, and do/don't guidance.

## Anti-Patterns

- Generic brand adjectives without concrete meaning.
- Inventing product facts when local context is thin.
- Replacing useful existing documentation.

## Acceptance Checklist

- Context files are specific to the product.
- Unknowns are clearly marked.
- Future Frontciti commands can use the files directly.
