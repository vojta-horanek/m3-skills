---
name: m3-components-dialogs
description: Design, implement, test, or verify Material 3 critical modal decisions, basic and full-screen dialogs, actions, errors, sizing, and focus cycles.
---

# Dialogs

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/dialogs/overview).

Use dialogs sparingly for critical information or a required decision.
Choose basic or full-screen dialogs for one task. Use snackbars for low-priority updates.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/dialogs/guidelines).

- Use clear headlines and action labels. Avoid ambiguous questions, alarms, and apologies.
- Provide at most two actions, one confirming and one dismissing.
- A single action must acknowledge information.
- Place confirmation nearest the trailing edge. Keep dismissal enabled.
- If basic-dialog confirmation requires a choice, disable it until that choice exists.
- Prefer adjacent buttons. If stacked, place confirmation above dismissal.
- Do not add a third action that leaves the dialog task unfinished.
- Use full-screen dialogs only at compact breakpoints.
- Use Save for saved selections or a clear action such as Create for completion.
- Full-screen confirmation should not open another dialog unless it fails.
- Confirm discarding unsaved full-screen changes with a basic dialog.
- Show field errors inline and all at once. Use basic dialogs for general submission failures.
- Pin title and buttons when content scrolls.
- Do not let background content scroll with the dialog.

## Implement the specs

Source: [Specs](https://m3.material.io/components/dialogs/specs).

- Basic dialogs use 28dp corners, dynamic height, and widths from 280 to 560dp.
- Use 24dp outer padding, 8dp button gaps, and 24dp between body and actions.
- Use 16dp between title and body and between icon and title.
- Icons measure 24dp.
- Center-align content with an icon. Start-align it without one.
- Use surface container high and a scrim.
- Full-screen dialogs use square corners and a 56dp header.
- On large screens, custom placement must respect 56dp edge margins.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/dialogs/accessibility).

- Place initial focus on the first interactive element.
- Cycle Tab and Shift+Tab through the dialog's interactive elements.
- Space or Enter activates the focused action. Escape closes the dialog.
- Keep focus in the dialog until dismissal or completion.
- Use the headline for the accessibility label.
- On web, use the alert-dialog role for basic dialogs.
- Label contained controls according to their own guidance.
- At 200% Android text size, keep headlines within four lines.
- If they truncate, expose the full content through one tap.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
