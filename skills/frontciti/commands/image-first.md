# /frontciti image-first

## Purpose

Use generated or supplied visual references as the art-direction source before coding visually important frontend work.

## Use When

Use for premium landing pages, creative sites, hero sections, portfolios, marketing pages, and redesigns where visual quality matters and image generation or strong visual references are available.

## Inputs To Inspect

Brief, desired section count, visual references, brand/product context, existing assets, generated images, screenshots, and implementation constraints.

## Workflow

1. Infer section count and visual goals.
2. Generate or gather one clear reference per section when helpful.
3. Generate detail views when typography, buttons, spacing, or components are too small to inspect.
4. Analyze each reference for text, type, spacing, color, layout, components, imagery, and rhythm.
5. Extract a design system from the references.
6. Implement faithfully without drifting into generic code templates.

## Output Expectations

The coded result should preserve the reference's hierarchy, spacing logic, palette, component family, and signature visual moves while remaining semantic, responsive, and accessible.

## Anti-Patterns

- One tiny unreadable board for many sections.
- Cropping old images instead of generating clear section references.
- Replacing strong references with generic card rows.
- Treating mock text as final copy when it is unreadable or inaccessible.

## Acceptance Checklist

- References are analyzable.
- Details are extracted before coding.
- Implementation stays faithful but production-safe.
