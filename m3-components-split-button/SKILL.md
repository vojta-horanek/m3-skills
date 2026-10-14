---
name: m3-components-split-button
description: Design, implement, test, or verify Material 3 primary actions with related menus, leading and trailing buttons, menu placement, and expanded states.
---

# Split buttons

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/split-button).

Use a split button to combine one main action with a menu of related actions.
Choose XS, S, M, L, or XL sizes and elevated, filled, tonal, or outlined colors.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/split-button).

- Keep the leading action label to one or two words.
- The leading button can contain text, an icon, or both.
- Keep the trailing expand/collapse icon unchanged.
- Mirror the component layout for RTL languages.
- Scale size to suit the breakpoint and action emphasis.
- Use the standard motion scheme for menu-button rotation.
- Rotate the menu icon inward by 180 degrees on opening and closing.
- Prefer aligning the menu with the trailing button.
- If space prevents this, align the menu with an edge of either button.
- Keep the menu 4dp from the split button.
- Avoid unusual changes to the menu.

## Implement the specs

Source: [Specs](https://m3.material.io/components/split-button).

- Use size-specific split-button tokens and standard button color tokens.
- Keep 2dp between the leading and trailing buttons.
- Use inner radii of 4, 4, 4, 8, and 12dp for XS through XL.
- Offset unselected menu icons from center by -1, -1, -2, -3, and -6dp for XS through XL.
- Center the icon normally when the trailing button is selected.
- Apply state layers on selection. Do not apply toggle-button color changes.
- Implement enabled, disabled, hovered, focused, pressed, and selected trailing-button states.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/split-button).

- Give each button a target of at least 48×48dp.
- Expand target height for XS and S buttons.
- Focus the leading button before the trailing button, subject to operating-system settings.
- Support Tab navigation and Space or Enter activation.
- Label the leading action according to button guidance.
- Label the trailing action as related additional choices, such as More watch options.
- Expose whether the menu is expanded or collapsed.
- Follow menu accessibility directions for the opened menu.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
