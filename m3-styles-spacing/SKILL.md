---
name: m3-styles-spacing
description: Apply and verify Material 3 spacing units, padding, gaps, margins, adaptive spacing, density, and tokens.
---

# Spacing

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read [source details](references/source-map.md) for section links, source tables, diagrams, and token modules.

Source: [Spacing: Overview](https://m3.material.io/styles/spacing).

Source: [Spacing: Applying spacing](https://m3.material.io/styles/spacing/applying-spacing).

Source: [Spacing: Tokens](https://m3.material.io/styles/spacing/tokens).

## Apply spacing units

- Use the linear 8dp-based spacing system for component and page layouts.
- Treat md.sys.measurement.space100 as 8dp.
- Use spacing tokens for margins, padding, and gaps rather than hardcoded custom-layout values.
- Use supported nested values such as 2dp, 4dp, 6dp, and 10dp where needed.
- Add missing system units using the multiplier pattern, such as space225 = 18dp.
- The supplied spacing token implementation is Jetpack Compose only.

## Choose the spacing attribute

- Use padding for space inside an element.
- Use gaps between elements within a grid or container.
- Use margins outside an element.
- Prefer parent padding and gaps before child margins.
- Use margins for layouts or extra space beyond parent padding.
- Use horizontal, vertical, leading, trailing, top, and bottom positions.
- Swap leading and trailing edges for right-to-left languages.
- Name simple gaps horizontal or vertical.
- Name distinct complex gaps by their adjacent elements, such as icon-label gap.
- Use panes, spacers, and margins for page structure, then padding and gaps within panes.

## Adapt at the component level

- Apply adaptive and density logic to component spacing attributes.
- Map attributes to different system tokens by form factor.
- Adapt vertical padding for density settings.
- Preserve spacing by default when text scales to 200%.
- Customize a component mapping when its default spacing must change across the product.
- Tokenize repeated adaptive patterns when multiple components share the same spacing behavior.
- Use padding, margin, and gap names for new attributes rather than the older generic space names.

## Verify

Check padding, gaps, margins, RTL edges, supported form factors, density settings, and text at 200%.
Read the source token module before selecting values that the text does not provide.
