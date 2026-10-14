---
name: m3-styles-color-system
description: Design, implement, or verify Material 3 color generation, HCT, theme support, and user-controlled contrast.
---

# Color system

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read the [source manifest](../m3-styles-sources.json) for source coverage.
Open the supplied source pages for tables, diagrams, and token modules.

Source: [Color system: Overview](https://m3.material.io/styles/color/system/overview).

Source: [Color system: How the system works](https://m3.material.io/styles/color/system/how-the-system-works).

## Apply the system

- Assign semantic color roles to UI elements. Apply their design tokens rather than individual color values.
- Use one set of roles for both light and dark themes.
- For dynamic color, use Material Color Utilities to generate schemes from a source color.
- Obtain the source from wallpaper, in-app imagery, or a deliberate color selection.
- Generate five key colors: primary, secondary, tertiary, neutral, and neutral variant.
- Generate tonal palettes from key colors. Assign accessible tones to roles, then assign roles to UI elements.
- Treat lower tone values as darker. Tone 0 is black, and tone 100 is white.
- Use HCT to adjust hue, chroma, and tone independently where supported.
- Do not substitute HSL lightness or saturation values for HCT tone or chroma.
- Account for hue-dependent and tone-dependent limits on available chroma.

## Support contrast settings

- Support standard, medium, and high contrast through appropriate color roles.
- Apply contrast settings in both light and dark themes.
- Use paired roles for custom components, such as primary container and on primary container.
- Preserve the distinction between essential content and containers at high contrast.
- Check medium contrast against the source's 3:1 minimum.
- Check high contrast essential elements against the source's 7:1 ratio.
- Do not treat these scheme settings as replacements for text-specific contrast requirements.

## Verify

Check role mappings in both themes and all three contrast settings.
Check custom components with their intended foreground and background pairs.
