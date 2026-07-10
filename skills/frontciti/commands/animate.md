# /frontciti animate

## Purpose

Add purposeful animation to frontend interfaces.

## Use When

Use when motion can clarify state changes, guide attention, create a memorable marketing moment, or coordinate complex visual sequences.

## Inputs To Inspect

Existing animation libraries, framework boundaries, component lifecycle, scroll behavior, performance constraints, reduced-motion needs, and user task.

## Workflow

1. Define the purpose of motion.
2. Choose CSS, existing framework motion, or GSAP.
3. Prefer transform and opacity.
4. Use timelines for sequences.
5. Scope animation to components.
6. Clean up timelines, observers, and ScrollTriggers.
7. Respect `prefers-reduced-motion`.
8. Test that motion does not block content or harm usability.

## When To Use GSAP

Use GSAP for sequenced timelines, ScrollTrigger, pinned sections, scrubbed effects, SVG animation, advanced staggered motion, or coordination across many elements.

## Anti-Patterns

- Animation only because it looks interesting.
- Long intros that block content.
- Scroll hijacking.
- Animating layout-heavy properties without need.
- Ignoring reduced motion.

## Acceptance Checklist

- Motion has a purpose.
- Performance is acceptable.
- Reduced motion is supported.
- Cleanup is handled.
- Animation does not reduce usability.
