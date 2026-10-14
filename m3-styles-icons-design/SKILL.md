---
name: m3-styles-icons-design
description: Draw and verify Material 3 custom icons using grids, keylines, stroke metrics, and optical corrections.
---

# Icon design

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read the [source manifest](../m3-styles-sources.json) for source coverage.
Open the supplied source pages for tables, diagrams, and token modules.

Source: [Icons: Designing icons](https://m3.material.io/styles/icons/designing-icons).

## Draw clear icons

- Simplify icons for clarity. Avoid complex, overly literal imagery.
- Use bold geometric forms and one consistent visual style.
- Make icons face forward. Do not tilt them or imply dimensional perspective.
- Create standard icons at 24dp × 24dp and inspect them at 100% scale.
- Use a 20dp × 20dp live area with 2dp perimeter padding.
- Extend into padding only for additional visual weight. Never exceed the trim area.
- Place icons on integer pixel coordinates.
- Use the source keyline template when the existing symbol library lacks the required icon.

| Keyline | Dimensions |
| --- | --- |
| Square | 18dp × 18dp |
| Circle | 20dp diameter |
| Vertical rectangle | 16dp × 20dp |
| Horizontal rectangle | 20dp × 16dp |

## Apply metrics

- Use 2dp exterior corner radii by default.
- Keep outlined-style interior corners square.
- Do not round stroke corners on shapes 2dp wide or less.
- Round both interior and exterior corners for rounded symbols.
- Use 0dp interior and exterior corner radii for sharp symbols.
- Use a recommended 2dp stroke or regular weight 400.
- Keep stroke weights and squared stroke terminals consistent.
- Use geometric optical corrections for complex details without skewing the underlying forms.
- Treat the source's 1.5dp paperclip and mixed-stroke ramen icons as optical correction examples.
- Use 20dp icons for dense desktop layouts and 40dp or 48dp for larger displays or headline contexts.

## Verify

Check live area, trim limits, pixel alignment, keyline proportions, corners, strokes, and legibility at the intended size.
