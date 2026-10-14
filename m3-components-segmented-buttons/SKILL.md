---
name: m3-components-segmented-buttons
description: Design, implement, test, or verify Material 3 baseline single-select and multi-select segmented buttons and migration to connected button groups.
---

# Segmented buttons

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/segmented-buttons/overview).

For Material 3 Expressive, use connected button groups instead. Segmented buttons are no longer recommended.
For baseline interfaces, use two to five segments for simple choices.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/segmented-buttons/guidelines).

- Use single-select segments for one option, view switching, or sorting.
- Use multi-select segments when any number of options, including none, can be selected.
- For more than five choices or complex choices, consider chips.
- Keep labels short and similar in length.
- Use one consistent label type across all segments.
- Do not mix icon-only segments with text-labeled segments.
- Do not wrap segments to another row.
- Use icon-only labels only when their meaning is clear.
- Keep margins around the container.
- Avoid spanning the full width of large screens with excessive segment padding.
- When a segment contains both icon and text, replace the icon with a checkmark on selection.

## Implement the specs

Source: [Specs](https://m3.material.io/components/segmented-buttons/specs).

- Use a 40dp container height and 48dp target size.
- Let container width follow labels and divide it equally among segments.
- Use a 1dp outline and centered labels.
- Keep left and right padding at least 12dp.
- Use 8dp between internal elements.
- Baseline density changes height in 4dp steps.
- Apply selected and unselected color roles and their interaction states.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/segmented-buttons/accessibility).

- Provide at least 3:1 outline contrast against the surface.
- Combine checkmarks and color to indicate selection.
- Start focus on the first segment, regardless of selection state.
- Place the first segment according to language direction.
- Support Tab entry, arrows between segments, and Space or Enter activation.
- Match accessibility labels to visible text or describe icon-only choices.
- Use radio-group semantics for single selection and checkbox semantics for multiple selection.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
