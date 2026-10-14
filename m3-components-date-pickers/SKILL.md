---
name: m3-components-date-pickers
description: Design, implement, test, or verify Material 3 docked and modal dates, date ranges, manual entry, formatting, calendar focus, and labels.
---

# Date pickers

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/date-pickers/overview).

Use docked, modal, or modal-input date pickers for dates and date ranges.
Clearly distinguish today's date, selected dates, and range endpoints.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/date-pickers/guidelines).

- Prefer full-screen modal selection in compact windows and docked selection in larger windows.
- For distant dates, use docked or modal input instead of a modal calendar.
- Support both keyboard entry and calendar selection in docked pickers.
- Use edit and calendar icons to switch modal input methods.
- Navigate single-date modal months horizontally and years through vertical year selection.
- Select a range by its start and end dates. Scroll range months vertically.
- Show connected highlighting between selected range endpoints.
- Place docked calendars below their fields.
- Confirm with OK or dismiss with Cancel. Full-screen pickers also provide Close and Save.
- Do not responsively enlarge picker dimensions.

## Implement the specs

Source: [Specs](https://m3.material.io/components/date-pickers/specs).

- Use the supplied token sets for docked, modal, and modal-input layouts.
- Preserve separate selected, today, outside-month, and in-range appearances.
- Modal containers use surface container high.
- Include enabled, disabled, hovered, focused, and pressed date and year states.
- Keep day, month, and year selection configurations distinct.
- Use the linked diagrams for measurements that the page supplies only as images.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/date-pickers/accessibility).

- Keep targets at least 48×48dp. Do not reduce their density.
- Provide manual date entry. Make calendar opening optional through the calendar icon.
- Give each input its own tab stop.
- Format after Enter or focus departure. Do not insert input-mask characters while typing.
- Accept dashes, spaces, slashes, dots, and leading zeros.
- Provide at least 4.5:1 date-text contrast against the background.
- Label the input's purpose and describe its expected format in helper text.
- Announce full dates, not day numbers alone.
- Include shortcut keys in tooltips and their screen reader hints.
- Remove unnecessary Clear actions to reduce tab stops.
- Enter saves the date and closes the calendar.
- Page keys change months. Shift with Page keys changes years.
- Shift+M and Shift+Y reach month and year dropdowns.

## Source limits

The keyboard table lists both Home and End as moving to the first day. Its first Enter row repeats Enter.
Do not infer distinct actions from these rows.
The guidelines mention time pickers in the date-picker dismissal paragraph. Treat that wording as a source error.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
