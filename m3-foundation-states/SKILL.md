---
name: m3-foundation-states
description: Design, implement, or audit Material 3 enabled, disabled, hover, focus, press, and drag states and state-layer values.
---

# Interaction states

## State meanings

Source: [States overview](https://m3.material.io/foundations/interaction/states/overview).

- Apply states consistently across components.
- Provide two visual indicators for states to support accessibility, as stated by the overview.
- States can combine, such as selection with hover.

| State | Meaning |
| --- | --- |
| Enabled | Interactive |
| Disabled | Inoperable |
| Hover | Cursor above an interactive element |
| Focused | Highlighted through input such as keyboard or voice |
| Pressed | User-initiated activation |
| Dragged | Pressed and moved |

## State layers

Source: [State layers](https://m3.material.io/foundations/interaction/states/state-layers).

- Put the semi-transparent state layer between the container and content.
- Use the content color, typically its corresponding “on” role, for the layer.
- If an icon is present, its content color supplies the default layer color. Otherwise use the label's color.
- Apply the layer to the whole element or as a circular shape, as appropriate.
- Apply only one state layer at a time, even when semantic states combine.
- Distinguish the layer from the interactive target. The source illustrates a 40dp layer within a 48dp target.

| State layer | Opacity |
| --- | --- |
| Hover | 8% |
| Focus | 10% |
| Press | 10% |
| Drag | 16% |

## Behavior

Source: [Applying states](https://m3.material.io/foundations/interaction/states/applying-states).

- Use the component's default style for enabled state.
- Show disabled state through color changes and reduced elevation. Disabled states are exempt from contrast requirements.
- Disabled controls cannot be focused, dragged, or pressed. They do not change state on tap or hover.
- Hide a FAB whose action is unavailable instead of displaying a disabled FAB.
- Use a low-emphasis animated fade for hover entry and exit.
- Show a ring-like indicator for keyboard focus. Permit keyboard action on the focused element.
- Use a high-emphasis ripple for pressed state. Some components can also use elevation.
- Keep dragged state low emphasis. Some draggable components can use elevation.
- Apply interaction states to actionable children rather than an entire app bar or other non-interactive container.
- A layout can contain many disabled elements, but only one hovered, focused, pressed, or dragged element for each respective state.
- Hover can combine with focus, activation, selection, or press.
- Focus can combine with hover, activation, or selection.
- Press can combine with hover, focus, activation, or selection.

Read [component applicability](references/component-applicability.md) when deciding which components inherit a state.

## Verify states

Check state meaning, input behavior, visual feedback, opacity, and layer color.
Check that disabled components remain inoperable and do not acquire interaction layers.
