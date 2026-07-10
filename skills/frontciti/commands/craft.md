# /frontciti craft

## Purpose

Shape, design, implement, inspect, and refine a frontend feature end to end.

## Use When

Use when the user wants a real shipped-quality build, not just a plan, critique, or small patch.

## Inputs To Inspect

Confirmed brief or `/frontciti shape` output, product/design context, existing files, stack, routes, components, tokens, assets, tests, and dev server behavior.

## Workflow

1. Load context and confirm the target surface.
2. If direction is ambiguous, run `/frontciti shape` first.
3. If visual quality is central and image generation is available, run `/frontciti image-first` before code.
4. Build in passes: structure, visual system, states, motion/media, responsive behavior, accessibility, performance.
5. Inspect in browser/screenshots when possible.
6. Patch material defects and re-inspect.
7. Run relevant verification commands before claiming completion.

## Output Expectations

Real code following project conventions, with semantic markup, responsive behavior, accessible states, real content/assets where possible, and no dead scaffolding.

## Anti-Patterns

- Starting with code when the brief needs shaping.
- Replacing product requirements with decorative mockups.
- Shipping only happy-path desktop UI.
- Ignoring the existing design system.

## Acceptance Checklist

- Confirmed direction was followed.
- Core states are implemented.
- Responsive and accessibility basics are verified.
- Build/test/lint commands were run when available.
