# Visual Assets

Brand and marketing surfaces need real visual material. Product UI often needs real screenshots, data, charts, or component previews.

## Priority

1. Use project-provided assets when available.
2. Generate raster assets when image generation is available and visual quality is central.
3. Use verified real image URLs when appropriate.
4. Use clear placeholder slots only when no credible asset path exists.

Do not fill image-led briefs with colored rectangles, fake screenshots, or div-based product previews.

## Hero Visuals

Text plus a gradient blob is usually not enough. The hero should contain one strong visual signal:

- Product screenshot or live component preview.
- Generated product/lifestyle image.
- Real photography.
- Immersive media scene.
- Typography as the visual object, when justified by the brief.

## Screenshots

If showing product UI:

- Prefer a real screenshot or actual component preview.
- Use realistic data.
- Avoid fake dashboards made of decorative rectangles.
- If data is mock, make that clear in code comments or sample data naming.

## Logo Walls

For real brands, use real SVG logos from verified sources. For invented brands, create a simple consistent mark, not plain text wordmarks.

Logo walls should be logos only. Do not add category labels under each logo unless the information is genuinely necessary.

## Image Quality

- Use stable aspect ratios.
- Reserve dimensions to avoid layout shift.
- Provide meaningful alt text, or mark decorative images empty.
- Keep image treatment consistent across the site.
- Verify remote URLs before shipping.

## Avoid

- Broken image guesses.
- Repeated stock-photo clichés.
- Hand-rolled sketchy SVG illustrations as fallback.
- Photo-credit captions as decoration.
- Pills or labels overlaid on images unless they carry real information.
