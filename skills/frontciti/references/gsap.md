# GSAP Implementation

Use GSAP when animation needs timelines, runtime control, scroll-linked behavior, SVG/text animation, draggable/gesture behavior, or coordination across many elements.

## Core Rules

- Install from public npm: `gsap`; use `@gsap/react` for React when available.
- Register plugins once before use.
- Prefer transform aliases: `x`, `y`, `xPercent`, `scale`, `rotation`.
- Prefer `autoAlpha` when hidden elements should not receive pointer events.
- Use timelines for sequences instead of delay chains.
- Store tween/timeline handles when playback control is needed.
- Use `gsap.matchMedia()` for responsive and reduced-motion variants.

## React And Next.js

- Run GSAP only on the client.
- Prefer `useGSAP()` from `@gsap/react`.
- Pass a scope ref so selectors only target inside the component.
- Use `contextSafe()` for handlers that create animations after setup.
- If `useGSAP()` is unavailable, use `gsap.context()` inside an effect and return `ctx.revert()`.
- Do not call GSAP or ScrollTrigger during SSR.

## ScrollTrigger

- Register `ScrollTrigger` once.
- Put ScrollTrigger on a top-level tween or timeline, not on a child tween inside a timeline.
- Use `scrub` for scroll-linked progress or `toggleActions` for discrete play/reverse. Do not mix both on one trigger.
- For pinning, usually use `start: "top top"` and animate children, not the pinned element itself.
- Create triggers in page order or set `refreshPriority`.
- Call `ScrollTrigger.refresh()` after layout changes caused by images, fonts, or dynamic content.
- Remove `markers: true` before production.

## Horizontal And Sticky Patterns

For fake horizontal scroll:

- Pin the wrapper.
- Animate the inner track.
- Use `ease: "none"`.
- Set `end` from the travel distance.
- Do not animate the pinned element horizontally.

For sticky stacks:

- Pin each card or panel deliberately.
- Use the next card's arrival to scale/fade the previous one.
- Avoid hidden content or scroll traps.

## Performance

- Animate transform, opacity, and bounded effects.
- Avoid casual animation of width, height, top, left, margin, or padding.
- Use `stagger` for groups.
- Use `quickTo()` for frequently updated pointer-following values.
- Use `will-change` only on elements that animate.
- Avoid hundreds of active tweens/triggers without testing.

## Plugins

Common plugin choices:

- ScrollTrigger: scroll-driven animation.
- ScrollToPlugin: smooth scroll to elements or positions.
- Flip: layout state transitions.
- Draggable + Inertia: drag and momentum.
- Observer: normalized wheel/touch/pointer gestures.
- SplitText: word/line/character animation with accessibility care.
- DrawSVG/MorphSVG/MotionPath: SVG animation.

Use only what the effect requires.

## Avoid

- Global selectors without scope.
- Missing cleanup.
- `window.addEventListener("scroll")` for animation progress.
- ScrollTrigger markers in production.
- Animating layout-heavy properties for movement.
- GSAP for simple hover transitions CSS can handle.
