# /frontciti component

## Purpose

Design or improve a single component, section, card, modal, table, form, navbar, sidebar, hero, pricing block, or UI pattern.

## Use When

Use when the requested scope is a focused UI element rather than a full screen or flow.

## Inputs To Inspect

Neighboring components, design tokens, props/API shape, state management, accessibility needs, responsive constraints, and existing usage sites.

## Workflow

1. Identify the component's role in the user journey.
2. Match the local design system and code conventions.
3. Design required states.
4. Keep props and composition simple.
5. Add semantic HTML, keyboard behavior, and ARIA only where useful.
6. Make responsive behavior explicit.
7. Polish spacing, type, feedback, and copy.

## Output Expectations

Consider default, hover, focus, active, disabled, loading, empty, error, success, selected, expanded, and collapsed states.

## Anti-Patterns

- Over-general component APIs.
- Styling that clashes with surrounding UI.
- Missing keyboard or focus behavior.
- States that shift layout unexpectedly.

## Acceptance Checklist

- Component is reusable.
- States are complete enough for real use.
- Accessibility basics are covered.
- Styling matches the product.
- Behavior is clear.
