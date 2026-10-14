---
name: m3-styles-elevation
description: Design, implement, or verify Material 3 elevation levels, tonal separation, shadows, scrims, and component stacking.
---

# Elevation

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read the [source manifest](../m3-styles-sources.json) for source coverage.
Open the supplied source pages for tables, diagrams, and token modules.

Source: [Elevation: Overview](https://m3.material.io/styles/elevation).

Source: [Elevation: Applying elevation](https://m3.material.io/styles/elevation/applying-elevation).

Source: [Elevation: Tokens](https://m3.material.io/styles/elevation/tokens).

## Apply elevation

- Use elevation tokens to express relative distance on the z-axis.
- Preserve default resting elevation for Material components.
- Use a small number of elevation levels.
- Keep interaction elevation changes consistent across similar elements.
- Reserve levels 4 and 5 for interaction states such as hover and drag.
- Use levels 0 through 3 for resting states.
- Treat token levels as relative placement. Platforms determine their visual shadows.
- Use elevation level tokens instead of deprecated surface tint color.

| Level | Height |
| --- | --- |
| 0 | 0dp |
| 1 | 1dp |
| 2 | 3dp |
| 3 | 6dp |
| 4 | 8dp |
| 5 | 12dp |

Read the supplied elevation tokens page's component table before assigning a component level.

## Depict separation

- Make surface edges, overlap, and distance understandable.
- Use tonal differences by default to separate surfaces.
- Use different surface roles for overlapping containment areas.
- Do not tie surface color roles directly to elevation levels.
- Give interactive edges enough contrast to distinguish surfaces.
- Use shadows to protect elements over busy backgrounds or encourage interaction.
- Use small, sharp shadows for close surfaces and larger, softer shadows for greater distance.
- Place scrims beneath modals and expanded navigation menus to focus attention.
- Use the scrim color role at 32% opacity.

## Verify

Check default stacking, interactive elevation changes, floating-element contrast, and scrim opacity.
Use the level table rather than inconsistent measurements in illustrative hover examples.
