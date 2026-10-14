---
name: m3-styles-color-brand
description: Create, apply, export, or verify Material 3 static brand color schemes.
---

# Static brand color

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read the [source manifest](../m3-styles-sources.json) for source coverage.
Open the supplied source pages for tables, diagrams, and token modules.

Source: [Static: Custom brand](https://m3.material.io/styles/color/static/custom-brand).

## Create the scheme

1. Open Material Theme Builder in Figma.
2. Enable New theme color diagram and Generate State Layers in Settings.
3. Select + ADD NEW THEME from Current Theme.
4. Give the theme a short name for its color role prefix.
5. Select ADD THEME.
6. Select Custom, then Primary.
7. Enter the brand source hex value and select Apply.
8. If needed, set sources for Secondary, Tertiary, Error, Neutral, and Neutral Variant.

## Apply and develop

- Copy the scheme diagram into the destination file to make its local color styles available.
- Enable the M3 Design Kit for new design files.
- Apply brand roles to custom elements according to their intended use.
- Search for the theme name in the color style selector.
- For existing kit components, select the scheme and affected frames in Theme Builder, then select Swap.
- Replace remaining hex values and non-brand styles with corresponding theme roles.
- Export the scheme for Jetpack Compose, Android Views, Flutter, Web, or JSON.
- Maintain the brand scheme as a product-owned static scheme.

## Verify

Check accessible pairings in both light and dark themes.
Check that custom elements and interaction state layers use the brand scheme.
