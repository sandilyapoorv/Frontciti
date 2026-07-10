---
name: frontciti
description: Frontend design, redesign, SaaS UI, dashboard, landing page, component, product UI, design-system, accessibility, responsive, polish, critique, UX copy, visual direction, image-first design-to-code, and GSAP motion skill for AI coding agents. Use when Codex needs to build, shape, audit, critique, polish, harden, animate, optimize, adapt, typeset, colorize, or improve websites, web apps, admin panels, client portals, dashboards, forms, charts, onboarding flows, components, and production-ready frontend interfaces.
---

# Frontciti

Frontciti turns frontend requests into specific, polished, production-minded interfaces. It combines product thinking, visual taste, UX rigor, accessibility, responsive behavior, design-system discipline, and purposeful motion.

## Operating Principle

Do not create generic AI-looking UI. Every visible choice must fit the product:

- Layout should match the audience, workflow, register, and content density.
- Typography should express the brand or serve the task.
- Color should support hierarchy, state, mood, and meaning.
- Spacing should create rhythm, grouping, and confidence.
- Components should feel designed, not assembled from defaults.
- Motion should clarify, guide, or delight; never distract.
- Accessibility, responsive behavior, and real states are baseline requirements.

## Register Router

First decide the register.

- **Brand register**: landing pages, marketing pages, campaigns, portfolios, about pages, long-form brand content. Design is the product. Read `references/brand-ui.md`, `references/registers.md`, and usually `references/visual-assets.md`.
- **Product register**: SaaS apps, dashboards, admin panels, settings, tools, authenticated surfaces, data tables, forms. Design serves the task. Read `references/product-ui.md`, `references/registers.md`, and usually `references/interaction.md`.

If a surface mixes both, route by the page being edited, not by the company category.

## Command Router

If the user names a command, follow it. Otherwise infer the nearest mode and read its command file before acting.

- `/frontciti init`: read `commands/init.md`.
- `/frontciti shape`: read `commands/shape.md`.
- `/frontciti craft`: read `commands/craft.md`.
- `/frontciti landing`: read `commands/landing.md`.
- `/frontciti saas`: read `commands/saas.md`.
- `/frontciti dashboard`: read `commands/dashboard.md`.
- `/frontciti component`: read `commands/component.md`.
- `/frontciti redesign`: read `commands/redesign.md`.
- `/frontciti critique`: read `commands/critique.md`.
- `/frontciti audit`: read `commands/audit.md`.
- `/frontciti polish`: read `commands/polish.md`.
- `/frontciti animate`: read `commands/animate.md`.
- `/frontciti harden`: read `commands/harden.md`.
- `/frontciti design-system`: read `commands/design-system.md`.
- `/frontciti extract`: read `commands/extract.md`.
- `/frontciti bolder`: read `commands/bolder.md`.
- `/frontciti quieter`: read `commands/quieter.md`.
- `/frontciti distill`: read `commands/distill.md`.
- `/frontciti delight`: read `commands/delight.md`.
- `/frontciti layout`: read `commands/layout.md`.
- `/frontciti typeset`: read `commands/typeset.md`.
- `/frontciti colorize`: read `commands/colorize.md`.
- `/frontciti clarify`: read `commands/clarify.md`.
- `/frontciti onboard`: read `commands/onboard.md`.
- `/frontciti adapt`: read `commands/adapt.md`.
- `/frontciti optimize`: read `commands/optimize.md`.
- `/frontciti image-first`: read `commands/image-first.md`.

## Default Workflow

For non-trivial frontend work:

1. Read the brief and inspect the existing app before designing.
2. Identify register, product type, audience, primary task, conversion goal, brand tone, technical constraints, and existing design system.
3. Read `PRODUCT.md` and `DESIGN.md` when present. If missing and context is unclear, use `/frontciti init` or infer with clearly marked assumptions.
4. Choose the command mode and load relevant references.
5. For ambiguous or high-stakes builds, shape the UX before code. Do not skip user confirmation when a design direction is genuinely unresolved.
6. Implement with the existing stack and conventions.
7. Include relevant states: default, hover, focus, active, disabled, loading, empty, error, success, selected, expanded.
8. Verify responsive behavior, accessibility, copy, hierarchy, color contrast, performance, and motion before finishing.

## Design Read

Before major visual work, produce a concise internal design read:

- Page or surface kind.
- Audience and context.
- Register: brand or product.
- Visual lane or design system.
- Variance, motion, and density level.

Use this to avoid defaulting to centered heroes, generic card rows, AI gradients, repeated section eyebrows, fake dashboards, and placeholder copy.

## Implementation Rules

Use the project's existing stack and patterns.

Before adding a package:

- Check whether the project already has an equivalent dependency.
- Prefer native CSS, Tailwind, browser APIs, or existing project utilities for simple effects.
- Use official design-system packages when the brief clearly maps to them.
- Use GSAP for sequenced timelines, ScrollTrigger, SVG/text animation, pinned or scrubbed scroll effects, or advanced coordination.
- Support `prefers-reduced-motion` for animation.

For React and Next.js:

- Use semantic HTML and accessible labels.
- Respect SSR and client boundaries.
- Scope browser-only animation to client components.
- Prefer `@gsap/react` when available for GSAP work.
- Clean up timelines, observers, subscriptions, and triggers.

## References

Load only the references relevant to the task:

- `references/registers.md`: brand vs product routing.
- `references/design-philosophy.md`: core design judgment.
- `references/anti-slop.md`: patterns to avoid.
- `references/preflight.md`: final anti-slop and production checks.
- `references/design-systems.md`: official systems, tokens, Tailwind/shadcn guidance.
- `references/ui-ux-rules.md`: hierarchy, layout, interaction, states.
- `references/product-ui.md`: SaaS and app-screen guidance.
- `references/brand-ui.md`: marketing and landing page guidance.
- `references/visual-assets.md`: imagery, logos, screenshots, and placeholders.
- `references/image-first.md`: image-first design-to-code workflow.
- `references/typography.md`: font, scale, measure, and text hierarchy.
- `references/color.md`: palette strategy, OKLCH, contrast, theming.
- `references/layout.md`: spacing, rhythm, grid, density.
- `references/interaction.md`: states, focus, forms, modals, menus.
- `references/motion.md`: general motion design.
- `references/gsap.md`: GSAP implementation rules.
- `references/accessibility.md`: accessibility checklist.
- `references/resilience.md`: i18n, long content, edge cases, error recovery.
- `references/charts.md`: chart and data-visualization rules.
- `references/forms.md`: form UX rules.
- `references/responsive.md`: responsive design rules.
- `references/copy.md`: UX copy, labels, errors, empty states.

## Final Self-Audit

Before finishing, check:

- Does the register match the surface?
- Does the design match the actual product and user?
- Is hierarchy clear within a few seconds?
- Does it work on mobile, tablet, and desktop?
- Are interaction states visible and accessible?
- Are empty, loading, and error states handled where relevant?
- Is motion useful, performant, and reduced-motion-safe?
- Does it avoid generic AI design tells?
- Is the implementation consistent with the codebase?
