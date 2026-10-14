---
name: m3-components-buttons
description: Design, implement, test, or verify Material 3 default buttons, toggle buttons, labels, color styles, sizes, and interaction states.
---

# Buttons

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/buttons/overview).

Use default buttons for actions and toggle buttons for binary selection. Choose elevated, filled, tonal, outlined, or text colors.
Use XS, S, M, L, or XL sizes with round or square shapes.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/buttons/guidelines).

- Use filled buttons sparingly for important final actions, ideally one per page.
- Use tonal buttons when an outline gives a supporting action insufficient emphasis.
- Use outlined buttons for secondary actions on simple backgrounds.
- Use text buttons for the lowest-priority actions. Do not underline them.
- Reserve elevated buttons for backgrounds that require visual separation.
- Write action labels in sentence case, ideally one to three words.
- Keep normal labels visible on one line without truncation.
- Let width fit the label. Keep the icon and label grouped and centered during resizing.
- Put one optional icon before the label, according to language direction.
- Use outlined icons for unselected toggles and filled icons for selected toggles.
- If no filled icon exists, increase its weight.
- Keep selected and unselected label lengths similar.
- Preserve element order across breakpoints. Constrain overly long buttons on large screens.

## Implement the specs

Source: [Specs](https://m3.material.io/components/buttons/specs).

- Use the current size and color token sets. Toggle buttons do not support the text style.
- Prefer 16dp small-button padding. The older 24dp padding is no longer recommended.
- Use fully rounded corners for round buttons.
- Use square corner radii of 12, 12, 16, 28, and 28dp for XS through XL.
- Use pressed corner radii of 8, 8, 12, 16, and 16dp for XS through XL.
- Use the same pressed shape for round and square buttons of the same size.
- On selection, change round toggles to square and square toggles to round.
- Keep elevated buttons at elevation 1 when enabled and 0 when disabled.
- Implement enabled, disabled, hovered, focused, and pressed states.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/buttons/accessibility).

- Provide at least 3:1 contrast against the background for enabled buttons.
- Measure container contrast for elevated, filled, and tonal styles.
- Measure label contrast for outlined and text styles.
- Support Tab for focus and Space or Enter for activation.
- Match the accessibility label to the visible label. Add context when necessary.
- On Android at 200% text size, keep labels within two lines.
- If larger text truncates, provide the full content through one tap.
- Use the modified web motion curve when rapid repeated clicks are expected.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
