---
name: m3-components-tooltips
description: Design, implement, test, or verify Material 3 plain and rich context, positioning, transient and persistent behavior, focus, and tooltip roles.
---

# Tooltips

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/tooltips/overview).

Use plain tooltips for concise icon-only labels and rich tooltips for extra details or relevant actions.
Rich tooltips may contain a subhead, links, and up to two buttons.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/tooltips/guidelines).

- Do not hide critical information in a tooltip. Use a dialog when interruption is required.
- Plain tooltips are unnecessary when the element already has a visible label.
- Keep plain text brief and avoid multiple lines where possible.
- Keep rich subheads and action labels short.
- Include a subhead when a rich tooltip appears automatically.
- Prefer adjacent rich-tooltip buttons rather than stacked buttons.
- Place plain tooltips above their targets, or below app-bar targets.
- Default rich placement is below and to the right. Reposition to stay on-screen.
- Do not cover the parent element.
- Hover triggers desktop tooltips. Long press triggers mobile tooltips.
- Transient tooltips disappear 1.5 seconds after leaving the target.
- Opening a new tooltip closes the previous tooltip.
- Persistent rich tooltips open on click or page load and remain until another element is used.
- Do not use persistent rich tooltips on icon buttons.

## Implement the specs

Source: [Specs](https://m3.material.io/components/tooltips/specs).

- Plain containers measure 24dp high with 8dp padding.
- Plain colors use inverse surface and inverse on surface.
- Rich containers use surface container, on surface variant text, and primary action text.
- Rich padding is 12dp top, 8dp bottom, and 16dp horizontally.
- Place plain tooltips 4dp from bounded controls and 8dp from unbounded content.
- Adjust dynamic positioning in 8dp increments.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/tooltips/accessibility).

- Show context on hover or focus for actionable elements.
- Keep information visible long enough without disrupting the task.
- Do not block important information or prevent an action.
- Move rich-tooltip focus top to bottom through its interactive elements.
- Do not trap keyboard or screen reader focus. Permit linear page navigation.
- Tab reaches available buttons. Space or Enter activates them.
- Use the Tooltip role or its platform equivalent.
- Label contained elements according to their own guidance.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
