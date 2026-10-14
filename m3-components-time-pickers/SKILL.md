---
name: m3-components-time-pickers
description: Design, implement, test, or verify Material 3 dial and input time selection, clock formats, constrained layouts, targets, and field semantics.
---

# Time pickers

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/time-pickers/overview).

Use modal dial or input pickers for hours, minutes, and periods.
Provide manual input as an alternative to dial interaction.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/time-pickers/guidelines).

- Use separate hour and minute fields.
- For 12-hour formats, include AM/PM selection. Omit it for 24-hour formats.
- Respect the time-format option set outside the component, such as system settings.
- Let people select dial values by tapping numbers or dragging.
- Provide a keyboard icon to open input and a clock icon to return to the dial.
- Use Cancel to dismiss and OK to save.
- Retain modal focus until confirmation or dismissal.
- Adapt to horizontal orientation when height is limited.
- If the dial still cannot fit, use the input variant.
- Do not shrink dial density or add scrolling to fit a constrained viewport.
- Keep the picker fully visible above a scrim.
- The usage guidance does not recommend nuanced values such as stopwatch milliseconds.

## Implement the specs

Source: [Specs](https://m3.material.io/components/time-pickers/specs).

- Use 24dp container padding.
- Use 96×80dp dial-selection fields, or 114dp width for the vertical 24-hour configuration.
- Use a 256dp clock dial and a 48dp selector handle.
- Use an 8dp selector center and 2dp track width.
- Input fields measure 96×72dp.
- The input period selector measures 52×72dp.
- Dial period selectors measure 52×80dp vertically or 216×38dp horizontally.
- Use the dial or input color tokens and enabled, hover, focus, and pressed states.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/time-pickers/accessibility).

- Provide manual entry through the keyboard icon.
- Keep dial targets at least 48×48dp.
- Support Tab to enabled time slots and Space or Enter activation.
- Give hour and minute fields text-input roles and labels Hour and Minute.
- Label keyboard and clock buttons Toggle input picker and Toggle dial picker.
- Announce dial values with the value, unit, and total.
- AM/PM uses radio-button roles in Wiz and Compose, and checkbox roles in Android Views.
- Label Cancel and OK as buttons.

## Source limits

The accessibility use cases mention seconds and milliseconds, while usage rejects granular stopwatch selection.
Do not treat that use-case list as a requirement to add granular controls.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
