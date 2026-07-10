# /frontciti layout

## Purpose

Fix spacing, rhythm, grid, density, alignment, and visual hierarchy.

## Use When

Use when a UI feels cramped, sparse, repetitive, misaligned, monotonous, or visually weak even though colors and components are mostly acceptable.

## Inputs To Inspect

Spacing tokens, layout CSS, component structure, grids, containers, breakpoints, screenshots, content density, and neighboring surfaces.

## Workflow

1. Assess spacing, hierarchy, grid structure, rhythm, density, and responsive behavior.
2. Choose a spacing scale and container strategy.
3. Use Flexbox for one-dimensional layout and Grid for two-dimensional layout.
4. Group related elements tightly and separate unrelated groups generously.
5. Replace unnecessary cards with spacing, dividers, or grouping.
6. Verify squint-test hierarchy and mobile collapse.

## Output Expectations

Layout should feel more structured, readable, and intentional without unnecessary decoration.

## Anti-Patterns

- Equal spacing everywhere.
- Identical card grids across every section.
- Nested cards.
- Arbitrary spacing values outside the project scale.
- Complex flex percentage math where grid would be clearer.

## Acceptance Checklist

- Primary hierarchy is obvious.
- Spacing follows a scale.
- Layout adapts cleanly.
- Density matches the task.
