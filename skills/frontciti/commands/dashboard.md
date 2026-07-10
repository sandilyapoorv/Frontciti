# /frontciti dashboard

## Purpose

Design dashboards, admin panels, analytics pages, reports, metric views, tables, and operational screens.

## Use When

Use when the UI helps users monitor state, compare data, make decisions, or take operational action.

## Inputs To Inspect

Metrics, chart data, reporting periods, user decisions, alerts, filters, table schemas, permissions, and existing analytics components.

## Workflow

1. Identify the decisions the dashboard supports.
2. Prioritize metrics by importance and urgency.
3. Group information by workflow.
4. Use cards, charts, tables, filters, and alerts intentionally.
5. Add search, sorting, date ranges, and row actions where useful.
6. Include empty, loading, error, and permission states.
7. Validate mobile and tablet behavior.

## Output Expectations

Every metric needs a label, value, unit, and context. Every chart needs a clear purpose. Alerts should be actionable.

## Anti-Patterns

- Vanity metrics with no decision value.
- Decorative charts with unclear units.
- Dense screens with no scan path.
- Tables without filters or actions.

## Acceptance Checklist

- A user quickly knows what needs attention.
- Metrics and charts are meaningful.
- Tables are usable.
- Filters are discoverable.
- Empty states guide action.
- The layout works at realistic density.
