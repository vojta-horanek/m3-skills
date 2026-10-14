---
name: m3-components-side-sheets
description: Design, implement, test, or verify Material 3 standard and modal side content, close controls, resizing, scrolling, RTL placement, and dialog semantics.
---

# Side sheets

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/side-sheets/overview).

Use side sheets for optional contextual content and actions.
Standard sheets leave main content interactive. Modal sheets require dismissal before returning to underlying content.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/side-sheets/guidelines).

- Prefer standard sheets in medium and expanded windows.
- Prefer modal sheets in compact windows.
- Place sheets on the trailing screen edge, away from leading navigation.
- Use the left edge and reverse internal elements for RTL languages.
- Keep a close affordance available.
- Use optional Back navigation within the sheet where needed.
- When a standard sheet opens, reduce body width while preserving its trailing margin.
- Keep sheet and page scroll positions independent.
- Allow vertical scrolling only. Do not allow horizontal scrolling.
- Modal sheets can become standard sheets as the window grows.
- On Android predictive back, detach from top and bottom edges and scale toward the gesture.

## Implement the specs

Source: [Specs](https://m3.material.io/components/side-sheets/specs).

- Default maximum width is 400dp.
- Use 24dp start and end padding, or 16dp start padding with a modal back icon.
- Use 12dp between top elements.
- Detached margins are 16dp.
- Bottom actions are 72dp high with 16dp top and 24dp bottom padding.
- Modal corners use a 16dp radius.
- Use surface for standard containers and surface container low for modal containers.
- Use outline variant for dividers and on surface variant for headings and icon controls.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/side-sheets/accessibility).

- Always include a close affordance, as required by the accessibility page.
- Make internal actions reachable through keyboard or switch tab order.
- Show visible focus on actions.
- Support Tab to enabled icon buttons and Space or Enter activation.
- Use the Dialog accessibility role for the sheet.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
