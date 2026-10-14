---
name: m3-styles-color-adjustments
description: Customize Material 3 scheme inputs, dynamic algorithms, color fidelity, or static color harmonization.
---

# Color adjustments

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read the [source manifest](../m3-styles-sources.json) for source coverage.
Open the supplied source pages for tables, diagrams, and token modules.

Source: [Advanced customizations: Adjust existing colors](https://m3.material.io/styles/color/advanced/adjust-existing-colors).

## Adjust baseline inputs

- Set primary, secondary, tertiary, neutral, and neutral variant sources in Material Theme Builder.
- Keep primary and tertiary visually prominent.
- Use a complementary tertiary hue where appropriate.
- Conventionally, secondary, neutral variant, and neutral share primary's hue with progressively less chroma.
- Apply the generated roles using their standard relationships.

## Adjust dynamic output

- Specify hue and chroma rules for primary, secondary, tertiary, neutral, and neutral variant groups.
- Define a scheme variant and use Material Color Utilities to generate its role values.
- Define custom roles only when other Material color solutions cannot meet the need.

## Use fidelity and harmonization

- Toggle Match color in Theme Builder to evaluate fidelity for source colors.
- Fidelity adjusts tones to better match the input while retaining accessible contrast.
- In code, use the scheme's boolean fidelity control for the relevant roles.
- Pair foregrounds with corresponding on-colors after fidelity changes.
- Toggle harmonization for each added static color in its overflow menu.
- In code, use Material Color Utilities' Blend function for harmonization.
- Preserve semantic hue meaning when static colors shift toward primary.
- Do not harmonize colors whose appearance must remain consistent, such as brand colors.

## Verify

Compare fidelity enabled and disabled for custom baseline or static colors.
Check harmonized colors under varied primary schemes.
Check intended role pairs after every tone adjustment.
