# /frontciti harden

## Purpose

Make frontend work production-ready.

## Use When

Use before shipping or when a UI needs accessibility, responsive, performance, edge-state, or maintainability cleanup.

## Inputs To Inspect

Semantic HTML, keyboard paths, focus states, form labels and errors, contrast, breakpoints, loading/empty/error states, images, bundle impact, motion, and edge cases.

## Workflow

1. Check accessibility basics.
2. Verify keyboard and focus behavior.
3. Check mobile, tablet, and desktop layouts.
4. Add missing loading, empty, error, disabled, and success states.
5. Optimize images and avoid unnecessary bundle cost.
6. Confirm motion safety and cleanup.
7. Simplify implementation where maintainability suffers.

## Output Expectations

The interface should be safer to ship, easier to use, and less fragile under real content and device conditions.

## Anti-Patterns

- Treating hardening as visual-only polish.
- Ignoring keyboard behavior.
- Leaving optimistic happy-path-only UI.
- Adding dependencies for minor fixes.

## Acceptance Checklist

- No obvious accessibility regressions.
- Mobile, tablet, and desktop layouts work.
- Interactions have states.
- Forms are usable.
- Edge cases are handled.
- Implementation is maintainable.
