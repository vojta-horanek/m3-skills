---
name: m3-foundation-selection
description: Design, implement, or verify Material 3 selection indicators, touch selection mode, desktop checkboxes, and batch-selection gestures.
---

# Selection

Source: [Selection](https://m3.material.io/foundations/interaction/selection).

## Indicators

- Show selection through a checkmark, checkbox, surface color change, or a combination.
- Selection can apply to a whole component or to part of it.
- Support selection through tap, cursor, keyboard, or voice as applicable.
- Navigation bars, drawers, rails, and tabs use active indicators. Select only one item at a time in these components.
- Use the active indicator's component-specific color and shape.

## Touch selection

- Enter selection mode with a long press or a shortcut such as an avatar tap.
- The source also identifies two-finger touch as a selection method.
- After entering selection mode, tap additional items to select them.
- Exit by deselecting all selected items or taking a toolbar action.
- For batch selection, long press and drag across items.
- Do not assign long press and drag to batch selection when that combination already picks up and moves the same items.

## Desktop selection

- When selection is the primary activity, keep checkboxes visible.
- When selection is secondary, show the hovered item's checkbox.
- After one item is selected, show selection indicators for all items.
- Allow the revealed checkbox to be clicked to select its item.

## Verify selection

Check selected indicators, selection-mode entry and exit, and desktop checkbox visibility.
Check that batch selection does not conflict with the gesture used to move items.
