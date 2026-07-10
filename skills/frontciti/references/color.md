# Color

Color should be strategic, accessible, and consistent.

## Strategy

Pick a strategy before picking colors:

- **Restrained**: neutrals plus one accent. Product UI default.
- **Committed**: one saturated color carries a meaningful portion of the surface.
- **Full palette**: several named roles used deliberately.
- **Drenched**: the surface is the color. Brand/campaign only.

## Product Color

- Use semantic roles for primary, selected, success, warning, error, info, disabled, muted, border, and surface.
- Reserve accent for primary action, current selection, or state.
- Avoid heavy inactive color.
- Keep chart and status colors clear and labeled.

## Brand Color

- Palette is voice.
- Use a named reference or subject-world rationale.
- Do not pick colors from category reflex alone.
- Committed or drenched color is allowed when it supports the brand.

## OKLCH And Tokens

Use OKLCH when creating new palettes. Build neutral ramps with tiny chroma toward the brand hue, not generic warm or cool by reflex.

Token layers:

- Primitive color scale.
- Semantic usage alias.
- Component-specific token.

Dark mode should redefine semantic tokens, not scatter overrides everywhere.

## Contrast

Minimums:

- Body text: 4.5:1.
- Large text: 3:1.
- UI components and focus indicators: 3:1.

Gray text on colored backgrounds often fails. Use a darker shade of the background hue or an intentional text token.

## Avoid

- Purple-blue AI gradients by default.
- Random extra accents.
- Alpha-heavy palettes that make contrast unpredictable.
- Color as the only indicator.
- Side-stripe accent borders as a default pattern.
- Hard-coded colors in a tokenized project.
