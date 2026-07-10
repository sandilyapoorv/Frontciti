# Image-First Design To Code

Use this when visual quality is central and image generation or strong visual references are available.

## Workflow

1. Infer section count and fidelity.
2. Generate or collect clear reference images before coding.
3. Prefer one image per section over one compressed multi-section board.
4. Generate detail views when text, buttons, cards, or spacing are unclear.
5. Analyze each image systematically.
6. Extract the design system.
7. Implement faithfully in code.
8. Re-check that code did not drift into generic templates.

## Analyze Each Reference

Extract:

- Section purpose.
- Visible text.
- Typography mood, size relationships, line count, weight, and tracking.
- Spacing, gutters, padding, and section rhythm.
- Button hierarchy, shape, padding, and state implications.
- Component structure and card logic.
- Palette, surface colors, border logic, and shadows.
- Image treatment and media frames.
- Layout grid and responsive implications.
- Signature motifs.

If a detail is unclear, generate a clearer standalone view rather than guessing.

## Implementation Discipline

Preserve:

- Layout logic.
- Spacing rhythm.
- Color strategy.
- Type hierarchy.
- Component family.
- Section ordering.
- Image-to-text balance.
- Signature visual idea.

Adapt for:

- Semantic HTML.
- Accessibility.
- Real copy.
- Responsive behavior.
- Performance.
- Maintainability.

## Avoid

- Tiny unreadable boards.
- Cropping old images for detail extraction.
- Ignoring text in the reference.
- Replacing visual direction with default cards.
- Copying inaccessible mock behavior blindly.
