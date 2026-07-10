# /frontciti adapt

## Purpose

Adapt a frontend for different screen sizes, input methods, densities, and responsive constraints.

## Use When

Use when desktop works but mobile/tablet, touch, overflow, or adaptive layout behavior is weak.

## Inputs To Inspect

Breakpoints, containers, tables, nav, modals, forms, charts, images, touch targets, content overflow, safe areas, and text scaling.

## Workflow

1. Identify priority content and actions at each viewport.
2. Define mobile, tablet, and desktop structures explicitly.
3. Replace fragile widths with responsive constraints.
4. Give tables, charts, modals, and navigation dedicated mobile strategies.
5. Verify touch targets, overflow, and text wrapping.

## Output Expectations

The UI should compose differently where needed, not merely shrink.

## Anti-Patterns

- Assuming stacking is enough.
- Tiny tap targets.
- Desktop tables squeezed into mobile.
- `h-screen` hero bugs on mobile browsers.
- Horizontal overflow.

## Acceptance Checklist

- Mobile, tablet, and desktop are intentionally handled.
- Primary actions remain reachable.
- No content overflows.
- Touch interactions are usable.
