# Design Systems

Use the existing design system first. Add a new system only when the project lacks one or the brief clearly requires an official system.

## Official Systems

Use official packages when the brief maps directly to them:

- Microsoft or enterprise productivity: Fluent UI.
- Google or Material product: Material Web / Material 3.
- IBM-style enterprise analytics: Carbon.
- Shopify admin: Polaris.
- Atlassian or Jira-like product: Atlassian Design System.
- GitHub-style devtool or community: Primer.
- UK public sector: GOV.UK Frontend.
- US public sector: USWDS.
- Modern owned React components: shadcn/ui or Radix primitives.

Use one design system per project. Do not mix systems unless an existing codebase already does.

## Token Architecture

Prefer three layers:

1. **Primitive tokens**: raw values, such as color scales, spacing, radius, shadows, durations.
2. **Semantic tokens**: purpose aliases, such as `--color-primary`, `--surface-muted`, `--text-danger`.
3. **Component tokens**: component-specific aliases, such as `--button-bg`, `--input-border`, `--card-padding`.

Semantic tokens enable theme switching. Component tokens enable component tuning without changing primitives.

## Component States

Define states consistently:

- Default.
- Hover.
- Focus.
- Active.
- Disabled.
- Loading.
- Error.
- Success.
- Selected.
- Expanded/collapsed.

State priority: disabled, loading, active, focus, hover, default.

## Tailwind And shadcn

- Check Tailwind version before changing config.
- Use mobile-first utilities.
- Avoid arbitrary values unless they encode a real design decision.
- Customize shadcn defaults. Do not ship the default theme unchanged.
- Use Radix/shadcn primitives for dialogs, menus, popovers, tabs, commands, and forms when the project already uses them.
- Keep focus rings, labels, descriptions, and keyboard behavior intact.

## Extraction Rules

Extract only patterns used 3+ times with the same intent.

Good extraction targets:

- Repeated components.
- Hard-coded values that should become tokens.
- Repeated type styles.
- Repeated layout or form patterns.
- Repeated motion timing or easing.

Do not extract one-offs or create generic components with unclear purpose.
