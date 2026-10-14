---
name: m3-components-floating-action-button
description: Design, implement, test, or verify Material 3 FAB sizes, constructive primary actions, placement, transitions, and accessibility.
---

# Floating action buttons

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/floating-action-button/overview).

Use a FAB for the most important or common action. Keep it visible while content scrolls.
Choose FAB, medium FAB, or large FAB. Small FABs are no longer recommended.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/floating-action-button/guidelines).

- Use one FAB per screen. Some screens do not need one.
- Use FABs for constructive actions such as create, favorite, share, or start.
- Avoid destructive, minor, overflow, unclear, or toolbar actions.
- Use medium FABs for most situations and large FABs for stronger emphasis or larger windows.
- Use a clear filled icon. Show an action tooltip on web hover.
- Do not add badges, notifications, or duplicate actions already present elsewhere.
- Prefer lower-right placement in compact and medium windows.
- Consider a navigation rail near the upper left in expanded windows.
- Do not give individual cards their own FAB.
- Keep the FAB stationary during content scrolling.
- During tab or screen transitions, briefly remove it and restore it only when relevant.
- Keep its position consistent where possible.
- Use a container transform for expansion into related content or a FAB menu.

## Implement the specs

Source: [Specs](https://m3.material.io/components/floating-action-button/specs).

- Use the current size and color token sets.
- Use primary container with on primary container by default.
- Secondary and tertiary container pairs are also available.
- Expressive also supports primary, secondary, and tertiary with their on-color roles.
- Surface color FABs are no longer recommended.
- Implement enabled, hovered, focused, and pressed states.
- Use an 8% hovered state layer and 10% focused or pressed state layers.
- Hover elevation is 4.
- For non-default mappings, use the icon color for the state layer.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/floating-action-button/accessibility).

- Hide a FAB when its action is unavailable. Do not disable it.
- Provide at least 3:1 icon contrast against the container.
- Prioritize its position in the overall focus order.
- Consider showing the tooltip on keyboard focus.
- Do not completely obscure another action's focus indicator.
- Test upper-left placement with users on larger screens.
- Support Tab focus and Space or Enter activation.
- Label the action, such as Compose a new message.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
