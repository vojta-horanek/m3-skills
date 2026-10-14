---
name: m3-components-sliders
description: Design, implement, test, or verify Material 3 standard, centered, and range values, stops, inset icons, orientation, synchronized inputs, and keyboard control.
---

# Sliders

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/sliders/overview).

Use sliders for values along a range. Apply changes immediately.
Choose standard, centered, or range variants with horizontal or vertical orientation.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/sliders/guidelines).

- Use standard sliders from the start of a sequence and centered sliders around a middle default or zero.
- Use two handles for minimum and maximum range values.
- Avoid vertical range sliders because they add cognitive load.
- Show the full available range.
- Keep active and inactive tracks the same size.
- Mirror increasing horizontal values for RTL languages.
- Show only one range-handle value label at a time.
- If using a separate text field, synchronize it with the slider and place it next in tab order.
- Snap to predefined stops when that configuration is used.
- Avoid so many stops that adjustment becomes difficult.
- Inset icons are only for M, L, or XL standard sliders.
- Move the inset icon to the inactive track when the active track has insufficient space.
- Reserve XL sliders for prominent moments where the slider is the page's focus.

## Implement the specs

Source: [Specs](https://m3.material.io/components/sliders/specs).

- Track heights for XS through XL are 16, 24, 40, 56, and 96dp.
- Handle heights are 44, 44, 52, 68, and 108dp. Handle width is 4dp.
- Track corner radii are 8, 8, 12, 16, and 28dp.
- Value-label containers measure 48×44dp.
- M and L inset icons measure 24dp. XL icons measure 32dp.
- Use common and size-specific tokens.
- Larger presets are available in Android Views. Other platforms may require swapping size tokens.
- Include enabled, disabled, hovered, focused, and pressed states.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/sliders/accessibility).

- Focus the handle initially.
- Tab reaches it. Arrows adjust one value or stop.
- Space with arrows adjusts the configured interval.
- Home and End select the first and last values.
- Make inactive track ends identifiable with at least 3:1 contrast.
- Keep end stops unless the track already has this contrast, or use equivalent contrasting visual anchors.
- Use a Slider role and a label matching adjacent text.
- External icon controls use Button roles.
- Indicate interaction through handle-width change and visible values.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
