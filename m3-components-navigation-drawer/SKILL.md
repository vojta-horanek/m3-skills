---
name: m3-components-navigation-drawer
description: Design, implement, test, or verify Material 3 baseline standard and modal navigation drawers, destination grouping, dismissal, and migration to expanded rails.
---

# Navigation drawers

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/navigation-drawer/overview).

For Material 3 Expressive, replace navigation drawers with expanded navigation rails.
For baseline designs, use standard or modal drawers for many destinations or multiple navigation levels.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/navigation-drawer/guidelines).

- Use standard drawers in expanded, large, and extra-large windows.
- Use modal drawers when compact or medium space is limited.
- Put frequent destinations first and group related destinations.
- Keep one destination active.
- Place the drawer on the leading edge, reversing its side for RTL languages.
- Open modal drawers through an external action.
- Dismiss modal drawers by destination selection, scrim selection, or swiping toward their anchor edge.
- Use full-width dividers between destination groups, not individual destinations.
- Require concise text labels. Truncate when needed rather than wrapping or shrinking them.
- Use icons for every destination or none.
- Keep drawer scrolling independent of body content.
- On web below 320 CSS pixels, swap the drawer for a navigation bar.
- Avoid two simultaneous primary navigation components.
- The baseline source permits a modal drawer opened from a rail when hierarchy remains visually distinct.

## Implement the specs

Source: [Specs](https://m3.material.io/components/navigation-drawer/specs).

- Use a 360dp width and full-height container.
- Standard leading-to-trailing corner radii are 0, 16, 16, and 0dp.
- Icons measure 24dp.
- Active indicators measure 336×56dp with 28dp corner radii.
- Use 28dp horizontal content padding and 12dp indicator padding.
- Start-align labels.
- Use surface container low and secondary container for the active indicator.
- Include enabled, hovered, focused, and pressed states.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/navigation-drawer/accessibility).

- Start focus on the first destination.
- Use Tab entry, arrows between destinations, and Space or Enter selection.
- When applicable, selection moves focus to the newly opened section.
- Keep scrim dismissal available for modal drawers.
- Distinguish selected icons through fill and color, backed by an active indicator.
- Label destinations with their visible names and clarify ambiguity where supported.
- Android Views does not support the extra descriptive label or announce the role.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
