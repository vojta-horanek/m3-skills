---
name: m3-components-menus
description: Design, implement, test, or verify Material 3 temporary actions, vertical menus, grouping, submenus, slots, disabled items, and keyboard navigation.
---

# Menus

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/menus/overview).

Use menus for temporary action sets. Use toolbars for persistent actions.
Prefer expressive vertical menus for new designs. Choose standard or vibrant colors.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/menus/guidelines).

- Use vibrant menus sparingly for greater emphasis.
- Group related items with dividers or at most one or two gaps.
- Do not change gap sizes or use gaps in scrollable menus.
- On web, use dividers because gaps are unavailable.
- Keep unavailable conditional actions visible but disabled.
- Reposition menus to prevent clipping by screen edges.
- Place submenus beside their parent without overlap.
- Prefer submenus on large screens. They are unavailable on Jetpack Compose.
- Consider bottom sheets for longer mobile menus.
- Keep custom slots simple and preserve menu padding and interaction patterns.
- Do not add nested buttons, switches, or multiple actions to menu items.
- Show a persistent scrollbar when menu content scrolls.
- Multi-select menus remain open until dismissed.
- Keep the trigger's pressed state while its menu is open.

## Implement the specs

Source: [Specs](https://m3.material.io/components/menus/specs).

- Use current vertical-menu token sets for shape, color, states, and submenu motion.
- Standard colors are surface-based. Vibrant colors are tertiary-based.
- Include enabled, disabled, hovered, focused, pressed, and active submenu states.
- Custom slot targets must measure at least 48×48dp.
- For baseline menus only, width ranges from 112 to 280dp with 4dp corners.
- Baseline item height is 48dp, horizontal padding is 12dp, and icons measure 24dp.
- Baseline dividers are 1dp high with 8dp vertical padding.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/menus/accessibility).

- Focus the first item when a menu opens.
- Support Escape, outside selection, and system Back for dismissal.
- Space or Enter opens menus or selects items.
- Up and Down open a closed menu or move within an open menu.
- Left and Right open or close submenus.
- Letters move to the next item starting with that letter.
- Disabled items can receive focus but cannot be selected.
- Gaps and dividers cannot receive focus.
- Show selection through shape and color, preferably with another cue such as a checkmark.
- Default selected versus unselected contrast is 3:1.
- Match labels to menu-item text and hide redundant decorative icons.
- Web items use Menu item roles. Android items use generic actionable roles.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
