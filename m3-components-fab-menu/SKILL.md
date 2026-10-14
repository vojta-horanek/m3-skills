---
name: m3-components-fab-menu
description: Design, implement, test, or verify Material 3 FAB menu actions, anchoring, scrolling, platform behavior, and focus.
---

# FAB menus

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/fab-menu/overview).

Use a FAB menu for two to six related actions. Open it only from a FAB.
Use it instead of speed dials or stacked small FABs.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/fab-menu/guidelines).

- Keep actions closely related under one main action.
- Do not open a FAB menu from an extended FAB or another component.
- Do not use it when the FAB is paired with a toolbar or navigation rail.
- Keep the menu at the FAB's position and trailing edge.
- Mirror the layout and use left alignment in RTL languages.
- Match the primary, secondary, or tertiary menu set to the FAB color set.
- Keep labels visible and items sized to fit their contents.
- Keep icons unless removing one is necessary.
- Do not set fixed item widths, truncate labels, or change the rounded shapes.
- Anchor the transition at the FAB's top trailing corner.
- In short windows, let items scroll behind the close button.
- Keep the close button accessible.
- On web, use the menu component for the FAB's options.

## Implement the specs

Source: [Specs](https://m3.material.io/components/fab-menu/specs).

- Use one menu size with any FAB size.
- Use medium-button measurements for menu items.
- Keep the close button 56dp.
- Use 16dp FAB margins. Increase margins to 24dp in large and extra-large windows.
- Align the FAB and close button at their top trailing corner.
- On web, a 4dp gap between FAB and menu is recommended.
- Implement enabled, hovered, focused, and pressed states for close and item buttons.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/fab-menu/accessibility).

- Maintain targets of at least 48×48dp.
- Do not completely hide another actionable element's focus indicator.
- Keep initial focus on the close button when it replaces the FAB.
- Then navigate from the top item to the bottom item.
- Support Tab navigation and Space or Enter activation.
- On Android, label the close button Toggle menu with button role and expanded or collapsed state.
- Give Android items button roles and labels matching visible text.
- On web, follow FAB and menu accessibility directions.
- Label the web FAB with the menu it opens.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
