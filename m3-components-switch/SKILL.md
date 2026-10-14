---
name: m3-components-switch
description: Design, implement, test, or verify Material 3 immediate binary settings, independent controls, handle states, density, and labels.
---

# Switches

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/switch/overview).

Use switches for independent on/off settings. Make the state visible at a glance.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/switch/guidelines).

- Apply switch effects immediately without a Save action.
- Use a switch for one binary option, not opposing choices such as list versus map.
- Use a connected button group for opposing options.
- Use checkboxes for multiple related choices, especially when saving is required.
- Use radio buttons for a single option from a list.
- Do not replace an action button with a switch.
- Pair the switch with a short inline label describing its on-state effect.
- Do not put label text inside the switch.
- Optional handle icons must clearly indicate state, such as a checkmark and X.
- Avoid ambiguous non-binary icons.
- Move the handle to the opposite track end on toggling.
- Use the larger handle to indicate the on state.

## Implement the specs

Source: [Specs](https://m3.material.io/components/switch/specs).

- Use a 52×32dp track with a 2dp outline and fully rounded corners.
- Without an icon, the unselected handle measures 16dp.
- Selected or icon-bearing handles measure 24dp.
- Pressed handles measure 28dp.
- Use a 40dp state layer and 48dp target.
- Selected and unselected icons measure 16dp.
- Use on surface for labels and optionally on surface variant for supporting text.
- Include enabled, hovered, focused, pressed, and disabled states.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/switch/accessibility).

- Provide handle-size feedback for tapping, dragging, clicking, and hover.
- Do not apply density by default.
- If users choose density, keep reversal controls at least 48×48 CSS pixels.
- Tab focuses the switch handle. Space or Enter toggles it.
- Link the adjacent label so assistive technology reads its text and role.
- Prefer clearer visible text when a label is ambiguous.
- Add descriptive accessibility context when necessary.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
