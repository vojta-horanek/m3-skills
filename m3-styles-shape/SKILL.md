---
name: m3-styles-shape
description: Apply and verify Material 3 shapes, corner tokens, asymmetry, customization, and optical roundness.
---

# Shape and corner radii

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read [source details](references/source-map.md) for section links, source tables, diagrams, and token modules.

Source: [Shape: Overview & principles](https://m3.material.io/styles/shape).

Source: [Shape: Corner radius scale](https://m3.material.io/styles/shape/corner-radius-scale).

## Apply shape deliberately

- Use shape and typography together for consistent visual attributes.
- Use abstract shapes sparingly. Preserve clarity and avoid visual clutter.
- Do not assign a literal meaning or fixed function to one abstract shape.
- Use unconventional library shapes mainly for visual elements, imagery masks, and decorative UI.
- Avoid unconventional shapes on text-heavy containers.
- Use contrasting round and square shapes when they help express state or draw attention.

## Apply the corner scale

| Style | Radius |
| --- | --- |
| None | 0dp |
| Extra small | 4dp |
| Small | 8dp |
| Medium | 12dp |
| Large | 16dp |
| Large increased | 20dp |
| Extra large | 28dp |
| Extra large increased | 32dp |
| Extra extra large | 48dp |
| Full | Fully rounded |

- Apply styles through shape tokens.
- Use corner-value tokens for individual corners, including grouped components' inner corners.
- Use the same scale for symmetric and asymmetric shapes.
- Use full for fully rounded corners rather than the previous 50% definition.
- Keep shape styles consistent unless a hero moment or custom component needs customization.
- Change a style value to affect all mapped components without overrides.
- Remap a component's shape token to affect that component across the UI.
- If using cut corners, add padding to prevent content clipping.
- Avoid large or full corners on information-dense components.

## Adjust nested corners

- Do not give nested rounded objects identical radii.
- Calculate optical roundness as inner radius = outer radius − padding.
- Use the source example of 48dp − 14dp = 34dp as a calculation example.

## Verify

Check token mappings, inner corners, content clipping, nested roundness, and the purpose of abstract shapes.
