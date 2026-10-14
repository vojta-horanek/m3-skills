---
name: m3-components-toolbars
description: Design, implement, test, or verify Material 3 docked and floating action containers, emphasis, slots, placement, responsive overflow, and accessibility.
---

# Toolbars

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/toolbars/overview).

Use docked toolbars for persistent global actions and floating toolbars for contextual page actions.
Docked toolbars replace baseline bottom app bars.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/toolbars/guidelines).

- Do not show a navigation bar and toolbar at the same time.
- Keep only essential actions visible and place overflow at the trailing end.
- Emphasize one action using color, width, or a paired FAB.
- Avoid too many controls or inconsistent control types.
- Do not use square filled icon buttons in rounded floating toolbars.
- Keep docked toolbars at the bottom and full-width by default.
- Keep floating toolbars fully inside the window or pane.
- Horizontal floating margins are at least 16dp. Vertical margins are at least 24dp.
- On large screens, put vertical toolbars opposite a centered navigation rail.
- Use narrow or default icon widths in vertical toolbars.
- Avoid multiple toolbars in compact windows.
- Mirror directional controls and meaningful action order for RTL languages.
- On scroll, remain visible, exit, or collapse as appropriate.
- Do not collapse actions and move the toolbar off-page simultaneously.

## Implement the specs

Source: [Specs](https://m3.material.io/components/toolbars/specs).

- Default toolbar height is 64dp with centered elements and equal inner spacing.
- Outside padding is at least 16dp. The default docked inter-item padding is 32dp.
- Every control needs a target of at least 48×48dp.
- Standard containers use surface container. Vibrant containers use primary container.
- Use the appropriate icon-button color mappings inside each color style.
- Floating toolbars have elevation by default, removable on visually distinct backgrounds.
- Jetpack Compose implements floating toolbars separately from docked toolbars.
- Paired floating FAB support is built in on Compose. Other platforms add both components separately.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/toolbars/accessibility).

- Keep actions accessible when content scrolls or controls collapse.
- Focus the first interactive element.
- Use Tab or arrows between interactive elements and Space or Enter activation.
- Give the web container a Toolbar role.
- Mobile containers can remain generic.
- The container has no interaction by default.
- Label and implement each internal action according to its component guidance.

## Source limits

The general guidelines require bottom placement and straight docked corners.
The large-screen section permits rounded docked toolbars in other page positions. Keep that exception limited to its stated context.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
