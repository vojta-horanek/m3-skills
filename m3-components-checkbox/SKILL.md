---
name: m3-components-checkbox
description: Design, implement, test, or verify Material 3 multiple related options, parent-child selection, indeterminate states, targets, and labels.
---

# Checkboxes

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/checkbox/overview).

Use checkboxes when people can select multiple related options.
Keep labels easy to scan and selected items visually prominent.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/checkbox/guidelines).

- Use checkboxes for multiple options, sub-selections, or desktop on/off controls.
- Do not replace a list of related checkboxes with switches.
- Use radio buttons when only one option can be selected.
- Selecting a parent selects all children.
- Clearing a parent clears all children.
- Show an indeterminate parent when some, but not all, children are selected.
- Selecting an indeterminate parent selects all children.
- When a checkbox turns an item on or off, apply the action immediately.
- On larger screens, consider grouping related controls in a side sheet.

## Implement the specs

Source: [Specs](https://m3.material.io/components/checkbox/specs).

- Use an 18dp container and icon with a 2dp container corner radius.
- Center the icon.
- Use a 48dp target and a 40dp state layer.
- Use on surface for adjacent text labels in every interaction and selection state.
- Include enabled, disabled, hovered, focused, and pressed states.
- Preserve selected, unselected, indeterminate, and error configurations.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/checkbox/accessibility).

- Let people select either the checkbox or its text label.
- Expose selected, unselected, and indeterminate parent states.
- Allow child checkboxes to change independently.
- Do not apply density by default.
- If users choose a denser layout, keep reversal controls at least 48×48 CSS pixels.
- Link the adjacent label so assistive technology reads its text and the checkbox role.

## Source limits

The source keyboard table describes chips and chip deletion. It does not supply a reliable checkbox keyboard mapping.
Do not use that table as checkbox behavior.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
