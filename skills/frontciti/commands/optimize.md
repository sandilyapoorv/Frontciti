# /frontciti optimize

## Purpose

Diagnose and improve frontend performance that affects user experience.

## Use When

Use when UI feels slow, janky, heavy, layout-shifty, image-heavy, animation-heavy, or bundle-heavy.

## Inputs To Inspect

Bundle/dependency usage, images, fonts, animations, render paths, expensive effects, layout shifts, hydration, scroll handlers, and devtools or Lighthouse output where available.

## Workflow

1. Identify the user-visible performance problem.
2. Check images, fonts, bundle cost, animation cost, render loops, and layout shifts.
3. Prefer removing work over hiding it with loaders.
4. Optimize assets and lazy-load below-the-fold weight.
5. Keep animation on compositor-friendly properties and bound expensive effects.
6. Re-run relevant performance/build checks.

## Output Expectations

The UI should feel faster and smoother without compromising clarity or accessibility.

## Anti-Patterns

- Adding animation to hide slow UI.
- Heavy libraries for small interactions.
- Unbounded blur/filter effects.
- Scroll listeners that update React state every frame.
- Images without reserved dimensions.

## Acceptance Checklist

- Main bottleneck is identified.
- Obvious waste is removed.
- Motion and images are bounded.
- Verification was run where available.
