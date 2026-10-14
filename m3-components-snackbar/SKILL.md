---
name: m3-components-snackbar
description: Design, implement, test, or verify Material 3 non-blocking feedback, persistent actions, web alternatives, placement, timing, focus, and polite announcements.
---

# Snackbars

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/snackbar/overview).

Use snackbars for low-priority process updates without interrupting the current task.
They can auto-dismiss or remain until acted on.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/snackbar/guidelines).

- Show only one snackbar at a time. Do not stack them or place them side by side.
- Provide at most one process action, with an optional close affordance.
- Do not make a snackbar the only route to a core use case.
- Prefer one line of message text, or at most two in compact windows.
- Use a text button for actions. Avoid inline links, styled text, and decorative icons.
- Place the snackbar near the bottom without covering navigation, frequent targets, or FABs.
- Put it above the FAB.
- Keep placement consistent on wider screens.
- Snackbars without actions can auto-dismiss after 4–10 seconds, depending on platform.
- Snackbars with actions remain until action or dismissal.
- On web, duplicate auto-dismissed information inline near its triggering action, or make the snackbar persistent and actionable.
- Updated information can replace an outdated snackbar immediately.
- Do not animate other components with snackbar animations.

## Implement the specs

Source: [Specs](https://m3.material.io/components/snackbar/specs).

- Use inverse surface for the container, inverse on surface for text, and inverse primary for the action.
- Use a legible solid background. Only slight transparency is acceptable if text remains clear.
- In compact windows, grow from 48 to 64dp for one or two text lines.
- On wider screens, grow horizontally and aim for one line with an optional action.
- Keep message text and action colors distinct.
- Do not significantly change the container shape.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/snackbar/accessibility).

- Announce appearance without moving or trapping focus.
- On Android and web, use a polite live-region announcement.
- iOS 17 and later uses polite announcements by default.
- When shown at launch, announce after the page title.
- On web, document a shortcut for actionable snackbar focus, such as Alt+G.
- Tab navigates interactive elements. Escape dismisses a focused snackbar.
- Return focus to the triggering or next logical element.
- Do not fully cover actionable elements or their focus indicators.
- Keep actionable snackbars available until the person responds.
- Material Web does not yet provide this component. These directions also apply to custom snackbars.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
