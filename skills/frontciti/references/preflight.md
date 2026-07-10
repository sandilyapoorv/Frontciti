# Frontciti Preflight

Run this before declaring visually important frontend work complete.

## Product Fit

- Register is correct: brand or product.
- Audience, task, and desired action are clear.
- The design has one primary focus per view.
- The result does not look like a category-default AI template.

## Visual System

- One color strategy is used consistently.
- Accent colors have meaning and contrast.
- Radius, shadow, border, and surface rules are coherent.
- Typography has a clear role scale.
- Body text is readable and limited to comfortable measure where applicable.

## Layout

- Hero or primary screen fits the first viewport.
- Navigation fits one line on desktop or collapses deliberately.
- Multi-column layouts have explicit mobile fallbacks.
- Section rhythm varies without becoming random.
- Cards are used only when they create meaningful grouping.
- No nested cards.
- No horizontal overflow.

## Content

- Copy is specific and grammatically sound.
- No placeholder copy, fake precision, or vague claims.
- CTAs use consistent labels for the same intent.
- Errors explain what happened and how to recover.
- Empty states guide the next action.

## Interaction

- Buttons, links, inputs, menus, modals, tabs, and tables have appropriate states.
- Focus states are visible.
- Keyboard paths work.
- Touch targets are large enough.
- Forms have labels, helper text, validation, and accessible errors.

## Motion

- Every animation has a purpose: hierarchy, story, feedback, or state transition.
- Reduced motion is supported.
- Content is not hidden behind animation failure.
- ScrollTrigger markers and debug code are removed.
- GSAP timelines, triggers, and observers are cleaned up.

## Technical

- Imports exist in project dependencies.
- Images have dimensions and alt text where meaningful.
- Fonts load without major layout shift.
- Build/test/lint commands were run when available.
- No console logs, dead code, broken links, or unused scaffolding remain.
