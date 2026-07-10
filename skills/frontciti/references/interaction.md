# Interaction

Design the full state cycle.

## Core States

Every relevant interactive element needs:

- Default.
- Hover.
- Focus.
- Active.
- Disabled.
- Loading.
- Error.
- Success.

Keyboard users see focus, not hover. Touch users may see neither. Design each path.

## Focus

- Never remove focus without replacement.
- Use `:focus-visible` where appropriate.
- Focus rings need at least 3:1 contrast against adjacent colors.
- Restore focus when closing modals or drawers.

## Forms

- Labels are visible.
- Placeholders are examples, not labels.
- Helper text explains constraints.
- Validate at useful moments, usually blur or submit.
- Error messages sit near the field and explain recovery.
- Preserve input after errors.

## Menus And Dialogs

- Prefer native dialog/popover or accessible primitives when the project uses them.
- Escape closes.
- Focus is trapped for modal dialogs.
- Menus support arrow navigation where expected.
- Avoid clipping dropdowns inside overflow containers; use top layer, fixed positioning, portal, or anchor positioning.

## Destructive Actions

Undo is often better than a confirmation dialog. Use confirmation for irreversible, high-cost, or bulk actions.

## Avoid

- Hover-only functionality.
- Tiny touch targets.
- Generic spinners where skeletons would explain layout.
- Dead links.
- Custom controls with no keyboard behavior.
