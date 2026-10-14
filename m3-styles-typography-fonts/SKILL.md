---
name: m3-styles-typography-fonts
description: Choose and verify Material 3 fonts, variable font capabilities, script coverage, and fallback order.
---

# Fonts and fallback

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read the [source manifest](../m3-styles-sources.json) for source coverage.
Open the supplied source pages for tables, diagrams, and token modules.

Source: [Typography: Fonts](https://m3.material.io/styles/typography/fonts).

## Choose the font

- Use Roboto as the default Material 3 and Android typeface.
- Use Roboto Flex when its variable weights, widths, and other axes support the design.
- Do not assume Roboto Flex is already part of the default M3 type scale.
- Use Roboto Serif for comfortable reading across a range of sizes.
- Use Roboto Mono for code or vertically aligned numbers.
- Use Noto Sans as the compatible fallback for unsupported language scripts.
- Check glyph coverage. Roboto Flex supports Latin, Greek, and Cyrillic in the supplied source.

## Apply fallback protection

1. Try Roboto Flex.
2. Fall back to Roboto.
3. Fall back to the Noto Sans font collection.

Confirm fallback availability with the product and engineering teams.
Read the supplied fonts page for the listed font-axis capabilities.

## Verify

Check supported characters and visual consistency through each fallback font.
Do not assume every font provides the same variable axes.
