---
name: m3-foundation-accessibility-flow
description: Design, implement, or verify Material 3 focus order, keyboard traversal, dialog focus, and keyboard shortcuts.
---

# Accessible flow

Source: [Flow](https://m3.material.io/foundations/designing/flow).

## Focus and traversal

- Make primary and secondary journeys achievable without a traditional mouse or touchscreen.
- Reduce page complexity and order tab stops deliberately.
- Use predefined tab order unless a journey or custom component needs a different pattern.
- The default web order follows the DOM, generally left to right and top to bottom.
- Group use cases into primary and secondary journeys. Use their priority to guide flow decisions.
- Define initial screen focus and initial focus within components that contain multiple interactive elements.
- When a dialog opens, move focus into the dialog, to the appropriate interactive element.
- When a dialog closes or is canceled, return focus to its trigger.
- Define atypical traversal for custom layouts or components.

| Key | Typical behavior |
| --- | --- |
| Tab | Move between interactive elements |
| Shift + Tab | Reverse tab direction |
| Arrow keys | Move within a component, such as a menu or a group |
| Enter | Activate a link or button, or submit a focused form |

A collection can use one tab stop with arrow-key traversal among its sub-elements when the layout warrants it.

## Shortcuts

- Use combinations of at least two keys by default.
- Provide a tutorial, list, or help page for all custom shortcuts.
- For a single-key shortcut, provide at least one of these options, in the source's preference order:
  1. Remap it to include a non-printable key.
  2. Activate it only while the relevant component has focus.
  3. Allow it to be disabled as a temporary solution.

## Verify flow

Complete primary and secondary journeys with the specified keys.
Check initial focus, dialog entry, focus return, and any custom traversal.
Check single-key shortcut controls and shortcut documentation.
