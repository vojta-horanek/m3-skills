---
name: m3-components-navigation-bar
description: Design, implement, test, or verify Material 3 compact and medium top-level destinations, flexible bars, active indicators, label scaling, and focus.
---

# Navigation bars

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/navigation-bar/overview).

Use navigation bars for three to five equally important, stable top-level destinations in compact or medium windows.
Use the flexible navigation bar instead of the older baseline bar.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/navigation-bar/guidelines).

- Keep one destination active.
- Use vertical items in compact windows and horizontal items in medium windows.
- Do not use a navigation bar for tasks, fewer than three destinations, or more than five destinations.
- Keep labels visible, brief, and untruncated at normal size.
- Do not shrink labels to fit.
- Keep destination positions fixed. Do not scroll or reorder them.
- Use filled active icons and outlined inactive icons.
- If a filled icon is unavailable, increase its weight to semibold.
- Place the bar at the bottom with full window width.
- Do not cover it with a FAB or permanently obstruct it.
- Use rails at expanded and larger breakpoints.
- Preserve destination state when frequent switching requires it, or reset it when appropriate.
- Re-selecting the active destination returns its page to the top.
- Do not swipe between destinations.
- Do not hide the bar on scroll with an active screen reader.

## Implement the specs

Source: [Specs](https://m3.material.io/components/navigation-bar/specs).

- Use surface container for the flexible bar.
- Use secondary container for the indicator and on secondary container for its active icon.
- Use secondary for active labels and on surface variant for inactive icons and labels.
- Vertical item widths divide the available container equally.
- Horizontal item widths remain fixed with extra space at the bar ends.
- Apply 8% hover and 10% focus or pressed state layers.
- Expand active indicators along one axis from the icon center.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/navigation-bar/accessibility).

- Keep active and inactive icon contrast at least 3:1 against the container.
- Use filled icons and bold labels for selected destinations.
- Use outlined icons and medium labels for unselected destinations.
- Let bar height grow with enlarged labels while preserving padding.
- Show full labels through 2× text scaling. Wrapping is allowed for enlarged text.
- Start focus on the first destination.
- Tab moves between items. Space or Enter selects one.
- Match accessibility labels to destination names. Add context to ambiguous labels where the platform permits.
- Android Views does not support the described extra label context or announce the role.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
