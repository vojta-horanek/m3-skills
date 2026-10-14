---
name: m3-components-icon-buttons
description: Design, implement, test, or verify Material 3 default and toggle icon buttons, icon meaning, size, width, states, and tooltips.
---

# Icon buttons

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/icon-buttons/overview).

Use a clearly understood system icon. Choose default or toggle variants.
Available configurations include four color styles, five sizes, three widths, and two shapes.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/icon-buttons/guidelines).

- Use default buttons for actions such as opening menus or search.
- Use toggles only for actions with selected and unselected states.
- Use filled, tonal, outlined, or standard colors according to action emphasis.
- Use filled styles sparingly for key actions.
- Use similar sizes for actions with equal importance.
- Use filled icons for default buttons.
- Use outlined icons for unselected toggles and filled icons for selected toggles.
- If no filled icon exists, use semibold weight. Use bold if semibold gives insufficient change.
- Show selection through at least two properties, rather than color alone.
- Use only a few icon buttons together unless a toolbar or button group organizes them.
- On web hover, show a clear tooltip that describes the action, not the icon's name.

## Implement the specs

Source: [Specs](https://m3.material.io/components/icon-buttons/specs).

- Use XS, S, M, L, and XL heights of 32, 40, 56, 96, and 136dp.
- Choose narrow, default, or wide widths from the size token sets.
- Use fully rounded corners for round buttons.
- Square radii for XS through XL are 12, 12, 16, 28, and 28dp.
- Pressed radii are 8, 8, 12, 16, and 16dp.
- Round and square buttons share a pressed radius at each size.
- Selected toggles change round resting shapes to square, or square to round.
- Use an 8% hover layer and 10% focused or pressed layers.
- Include disabled states and the specified color roles for each variant.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/icon-buttons/accessibility).

- Give every icon button a target of at least 48dp, including buttons nested in other components.
- Expand XS and S target areas to at least 48×48dp.
- Provide at least 3:1 icon contrast against its surface or background.
- Do not apply density by default.
- If users can choose density, keep its reversal controls at least 48×48 CSS pixels.
- Support Tab focus on enabled buttons and Space or Enter activation.
- Use an action-based accessibility label.
- On web, provide a tooltip with a concise accessibility label.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
