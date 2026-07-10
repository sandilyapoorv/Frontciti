# /frontciti saas

## Purpose

Design SaaS product interfaces, app shells, onboarding, client portals, settings, billing, project flows, and product dashboards.

## Use When

Use when the interface is primarily for logged-in product use rather than marketing.

## Inputs To Inspect

Routes, navigation, user roles, workflows, tables, forms, settings, billing, onboarding, permissions, empty states, and existing design tokens.

## Workflow

1. Identify core workflows and user jobs.
2. Separate marketing needs from product UI needs.
3. Organize navigation around user intent.
4. Clarify primary, secondary, destructive, and recovery actions.
5. Add realistic empty, loading, error, success, disabled, and pending states.
6. Ensure dense screens remain scannable.
7. Make app shell behavior responsive.

## Output Expectations

Support real SaaS usage: dashboards, projects, clients, leads, pipelines, invoices, contracts, payments, reports, onboarding, settings, billing, and client portals as relevant.

## Anti-Patterns

- Marketing-style hero treatment inside operational screens.
- Navigation based on implementation details.
- Static tables with no actions.
- Empty states that do not tell the user what to do.

## Acceptance Checklist

- Main workflows are obvious.
- Navigation is scalable.
- Important statuses are visible.
- Lists and tables have useful actions.
- Forms include validation and helper text.
- Responsive behavior supports actual use.
