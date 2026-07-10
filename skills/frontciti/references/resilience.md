# Resilience

Production UI must survive real data, slow networks, translations, permissions, and errors.

## Test Inputs

Use:

- Very long names and titles.
- Empty strings.
- Single-character values.
- Large numbers.
- Many items.
- No items.
- Special characters, accents, emoji, CJK, and RTL text.
- German-length translations.

## Layout Resilience

- Use `min-width: 0` inside flex/grid children that contain text.
- Use truncation only when full text is available elsewhere.
- Use line clamps for summaries.
- Allow wrapping for user-generated content.
- Avoid fixed-width buttons for translated labels.

## Error Resilience

Handle:

- Offline and timeout.
- 400 validation.
- 401 login.
- 403 permission.
- 404 not found.
- 429 rate limit.
- 500 server failure.

Provide recovery: retry, edit, go back, contact support, or save draft.

## Internationalization

- Use logical properties where possible.
- Do not concatenate pluralized strings manually.
- Use `Intl.DateTimeFormat` and `Intl.NumberFormat` where applicable.
- Allow 30-40% text expansion.
- Check RTL layout if the product supports it.

## Avoid

- Perfect-data-only layouts.
- Buttons that break with longer labels.
- Tables that collapse under long values.
- Error states that blame the user.
- Disabled actions with no explanation.
