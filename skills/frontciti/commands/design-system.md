# /frontciti design-system

## Purpose

Create or improve a design system for a frontend product.

## Use When

Use when a project needs reusable rules for visual language, tokens, components, layout, accessibility, or future interface consistency.

## Inputs To Inspect

Existing CSS, Tailwind config, theme files, components, routes, screenshots, tokens, icons, typography, colors, spacing, radii, shadows, and motion.

## Workflow

1. Inspect existing styles and components.
2. Define the design personality.
3. Create tokens for color, type, spacing, radius, shadow, border, and motion.
4. Define component rules.
5. Define layout and responsive rules.
6. Define accessibility rules.
7. Document do/don't examples.
8. Update implementation where relevant.

## Output Expectations

Include color system, typography scale, spacing scale, radius rules, elevation rules, motion rules, component inventory, layout rules, responsive behavior, and accessibility checklist.

## Anti-Patterns

- Token names that encode one-off pages.
- Design rules unrelated to the actual product.
- Documentation that cannot be used in code.
- Rebuilding the whole UI just to define tokens.

## Acceptance Checklist

- Design system is specific.
- Tokens are usable in code.
- Components are documented.
- Rules reduce future inconsistency.
