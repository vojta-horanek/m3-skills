---
name: m3-components-radio-button
description: Design, implement, test, or verify Material 3 single-option groups, adjacent labels, opt-out controls, targets, and keyboard selection.
---

# Radio buttons

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/radio-button/overview).

Use radio buttons when one option can be selected from a visible list.
Keep labels easy to scan and the selected option prominent.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/radio-button/guidelines).

- Use radio buttons for five or fewer options when exposing the choices is useful.
- Consider a menu when space is constrained, while accounting for its extra interaction effort.
- Do not nest radio buttons or use them for multiple selection.
- Pair every option with its own clear adjacent label.
- Prefer vertical lists.
- Selecting either an icon or its label selects that option.
- Apply changes immediately unless the containing page or dialog requires saving.
- The guidelines recommend a preselected option.
- The accessibility page also permits an initially unselected group.
- After selection, do not deselect the group by selecting the active option again.
- Provide No, Not applicable, or a separate Clear selection action when opting out is necessary.

## Implement the specs

Source: [Specs](https://m3.material.io/components/radio-button/specs).

- Use 20dp icons, 40dp state layers, and 48dp targets.
- Use primary and on surface variant for the specified radio states.
- Use on surface for adjacent labels in all interaction states.
- Include enabled, hovered, focused, pressed, and disabled states.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/radio-button/accessibility).

- Do not apply density by default.
- If users choose density, keep its reversal controls at least 48×48 CSS pixels.
- Tab enters at the selected option, or the first option if none is selected.
- Shift+Tab enters at the selected option, or the last option if none is selected.
- Arrows move focus and selection, wrapping between first and last options.
- Space selects a focused option and does nothing when it is already selected.
- Label the group by its title and use the Radio group role.
- Label each option with its adjacent text.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
