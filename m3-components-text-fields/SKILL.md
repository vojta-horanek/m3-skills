---
name: m3-components-text-fields
description: Design, implement, test, or verify Material 3 filled and outlined input, labels, errors, read-only fields, counters, adaptive sizing, and accessibility.
---

# Text fields

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/text-fields/overview).

Use filled or outlined text fields for text entry. Both provide the same functionality.
Make input and error states clear, with brief labels and actionable errors.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/text-fields/guidelines).

- Keep one variant within a form or region. Separate variants by region if both are needed.
- Provide a short, always-visible label, or a clear adjacent label.
- Do not wrap or truncate labels.
- Mark required fields with an asterisk and explain it in supporting text or a form note.
- Use single-line fields for short input.
- Use multi-line fields for growing content and fixed-height text areas for longer web responses.
- Show counters when character or word limits apply.
- Replace supporting text with error text to reduce layout shifts.
- Explain how to avoid the likely error. Allow sufficient space for longer errors.
- Strongly prefer an error icon as an additional visual cue.
- Show Clear only when input exists.
- Clearly label read-only fields.
- Constrain large-screen field width with flexible margins or containers.
- Do not apply density by default.

## Implement the specs

Source: [Specs](https://m3.material.io/components/text-fields/specs).

- Default height and target size are 56dp.
- Use 16dp horizontal padding without icons and 12dp with icons.
- Use 16dp between icons and text.
- Vertically center icons.
- Use 4dp above supporting text and counters, and 16dp between them.
- Filled fields use 8dp vertical padding and surface container highest.
- Outlined populated labels use 4dp side padding.
- Use the current filled or outlined tokens for empty, populated, disabled, focused, hover, and error states.
- In-field images can measure 24dp high.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/text-fields/accessibility).

- Provide at least 3:1 outlined-container contrast against the background.
- Tab reaches enabled fields and interactive icons.
- Match the accessibility label to the field label.
- Label interactive trailing icons by their current actions, such as Show password or Hide password.
- Label non-actionable error icons Error.
- Give prefix and suffix descriptions unique IDs and meaningful expanded names.
- Give errors an Alert role with the error message.
- If both supporting and error text exist, announce supporting text first.
- Label counters with character-count meaning and label supporting text separately.
- Include the required-field asterisk in the accessibility label.
- Keep density-reversal targets at least 48×48 CSS pixels.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
