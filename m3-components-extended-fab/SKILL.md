---
name: m3-components-extended-fab
description: Design, implement, test, or verify Material 3 extended floating action buttons, primary actions, labels, placement, and responsive behavior.
---

# Extended FABs

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/extended-fab/overview).

Use an extended FAB for a screen's main action when text clarifies an ambiguous icon.
Material 3 Expressive provides small, medium, and large variants.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/extended-fab/guidelines).

- Show only one extended FAB per screen.
- Provide persistent access above long scrolling content.
- Do not use an extended FAB as one option in an action set.
- Use a label of one or two words. Account for longer translations.
- Do not wrap or truncate the label.
- Icons are optional. Do not use an extended FAB without a text label.
- Keep the icon and label's meaning consistent.
- Do not place extended FABs on cards, inside content containers, or over toolbars.
- Do not pair them with floating toolbars.
- In compact and medium windows, use bottom center or bottom trailing placement.
- In expanded windows, use the bottom right edge or the navigation rail.
- Mirror internal icon and label placement for RTL languages.
- Transform between FAB and extended FAB as space changes.
- On downward scroll, an extended FAB can collapse to a FAB. Reverse this on upward scroll.

## Implement the specs

Source: [Specs](https://m3.material.io/components/extended-fab/specs).

- Use small, medium, or large heights of 56, 80, or 96dp.
- Replace the baseline extended FAB with the small variant and its updated typography.
- Do not use the old surface color style for new Expressive designs.
- Use primary, secondary, or tertiary color pairs, including their container pairs.
- Apply the corresponding color tokens in light and dark themes.
- Maintain 16dp margins.
- Implement enabled, hovered, focused, and pressed states.
- For non-default mappings, use the icon color for the state layer.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/extended-fab/accessibility).

- Place the extended FAB where people can reach it without obstructing other actions.
- Consider upper-left placement in a large web navigation rail for screen reader access.
- Prioritize the extended FAB in the overall focus order.
- Treat its icon and visible label as one focusable element.
- No tooltip is required when its label is visible.
- Support Tab focus and Space or Enter activation.
- Start the accessibility label with the same word as the visible label.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
