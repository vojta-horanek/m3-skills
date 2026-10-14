---
name: m3-styles-color-application
description: Combine Material 3 color schemes or remap roles on existing and custom components.
---

# Advanced color application

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read [source details](references/source-map.md) for section links, source tables, diagrams, and token modules.

Source: [Advanced customizations: Overview](https://m3.material.io/styles/color/advanced).

Source: [Advanced customizations: Apply colors](https://m3.material.io/styles/color/advanced/apply-colors).

## Combine schemes

- Start with a baseline or user-generated scheme as a consistent foundation.
- Map content-based roles to contained spaces above that foundation.
- Use local content color to emphasize content, associate related items, or support immersive content experiences.
- Keep the source content visible where its content-based color appears.
- Limit a screen to two schemes from different source types.
- Do not replace semantic colors with content-based colors when this would obscure conventional meaning.

## Remap components

- Choose roles by use, intended expression, and required contrast.
- In Figma, select the element and open the color property's Style selector.
- Search for the theme and select the role matching the element's function.
- Repeat until the component uses scheme roles throughout.
- Apply roles rather than static values or tonal palette values.
- Pair each background with its corresponding on-color.
- Meet 4.5:1 contrast for small text and 3:1 for large text.
- If existing roles cannot meet the need, define new roles or adjust the scheme.

## Verify

Test remapped components in light and dark themes and red, yellow, green, and blue schemes.
Check semantic meaning, content-source visibility, and foreground/background pairings.
