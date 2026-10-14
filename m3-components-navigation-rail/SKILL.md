---
name: m3-components-navigation-rail
description: Design, implement, test, or verify Material 3 collapsed and expanded rails, modal navigation, destinations, FAB placement, label scaling, and focus.
---

# Navigation rails

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/navigation-rail/overview).

Use collapsed or expanded rails for medium through extra-large windows.
Collapsed rails replace baseline rails. Expanded rails replace navigation drawers in Material 3 Expressive.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/navigation-rail/guidelines).

- Keep collapsed rails visible on the leading edge, outside content panes.
- Show three to seven collapsed destinations.
- Use a menu icon to expand or collapse. Do not use a logo as that control.
- Standard expanded rails sit beside content. Modal rails overlap it when space is limited.
- A modal expanded rail can open from a menu in compact windows.
- Keep the menu and optional FAB top-aligned.
- Center destination groups on tablets when this improves reach.
- Use one active indicator for the current page.
- Require clear, preferably one-word labels. Do not truncate or shrink them.
- Mirror placement for RTL languages.
- Put expanded badges beside labels and collapsed badges at icon corners.
- Keep destinations fixed during vertical scrolling.
- Never show a rail and navigation bar simultaneously.
- Adjust body space as a standard rail expands.
- Transform its FAB to an extended FAB when expanded.

## Implement the specs

Source: [Specs](https://m3.material.io/components/navigation-rail/specs).

- Use the current rail and navigation-item token sets.
- Expanded item targets span the entire rail width even when indicators fit their contents.
- Use surface container optionally, secondary container for the active indicator, and on secondary container for active icons.
- Vertical active labels use secondary. Horizontal active labels use on secondary container.
- Use on surface variant for inactive icons and labels.
- Nested FAB resting elevation is 0.
- Implement enabled, hovered, focused, and pressed states.
- Predictive back applies only to modal expanded rails.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/navigation-rail/accessibility).

- Use default colors with sufficient icon contrast. Limit destination colors to two.
- If container fill is removed, maintain at least 3:1 item contrast.
- Use filled active icons or semibold weight if no filled icon exists.
- Grow items vertically for enlarged labels while preserving padding.
- Keep complete labels visible through 2× text size. Scaled text can wrap.
- Focus the first interactive element, which may be Menu, FAB, or a destination.
- Use Tab or arrows to navigate and Space or Enter to activate.
- Match destination accessibility labels to visible names and clarify ambiguity where supported.
- Android Views does not support the extra descriptive label or announce the role.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
