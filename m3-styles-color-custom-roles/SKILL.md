---
name: m3-styles-color-custom-roles
description: Define and verify Material 3 additional static colors, semantic colors, and custom dynamic color roles.
---

# Additional colors and custom roles

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read the [source manifest](../m3-styles-sources.json) for source coverage.
Open the supplied source pages for tables, diagrams, and token modules.

Source: [Advanced customizations: Define new colors](https://m3.material.io/styles/color/advanced/define-new-colors).

## Define additional static colors

- Use Material Theme Builder to derive four roles from a reference color.
- Use the main, on-main, container, and on-container roles with the same relationships as standard accent roles.
- Use these roles for semantic or brand needs within a dynamic scheme.
- Use the provided Error roles for semantic red errors.
- Try color fidelity when generated tones differ from the intended source appearance.
- Optionally harmonize static colors with the primary hue while preserving semantic meaning.
- Keep colors unharmonized when literal sources require consistent appearance, such as signage or brand colors.

## Define custom roles only when other solutions cannot meet the need

1. Select a Material palette for each role.
2. Specify reference tones for both light and dark themes.
3. Specify foreground/background pairings and any required tone deltas.
4. Confirm that each pairing meets Material contrast minimums.
5. Define the roles in a dynamic color object.
6. Call Material Color Utilities to generate values for user themes and contrast conditions.

Use primary, secondary, tertiary, neutral, neutralVariant, or error as the reference palette.

## Verify

Check role pairings, reference tones, and contrast in both themes and supported dynamic conditions.
