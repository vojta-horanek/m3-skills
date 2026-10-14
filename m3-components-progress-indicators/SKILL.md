---
name: m3-components-progress-indicators
description: Design, implement, test, or verify Material 3 linear and circular progress, determinate accuracy, track ends, placement, and progress announcements.
---

# Progress indicators

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/progress-indicators/overview).

Use linear or circular indicators for ongoing processes. Keep a process's configuration consistent across the product.
Choose determinate or indeterminate behavior, flat or wavy shape, and default or configurable thickness.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/progress-indicators/guidelines).

- Use one indicator for a group of activities, rather than one per item.
- Under 200ms, use no indicator. For 200ms to 5s, prefer loading indicators.
- For longer waits, use progress indicators and consider allowing navigation away.
- Represent known progress accurately from 0% to 100%.
- Use indeterminate behavior when progress is unknown.
- Change indeterminate progress to determinate when reliable progress becomes available.
- Place linear indicators on the affected container's edge and circular indicators at its center.
- Place additional-item loading feedback in empty space, without covering current content.
- In buttons, match the active indicator to label or icon color and remove the track.
- Prefer flat indicators in very small buttons.
- Mirror linear indicators for RTL languages. Do not mirror circular indicators.

## Implement the specs

Source: [Specs](https://m3.material.io/components/progress-indicators/specs).

- Use primary for the active indicator and secondary container for the track.
- Default track thickness is 4dp.
- Use a 4dp stop circle for linear determinate progress when the track lacks 3:1 surrounding contrast.
- Do not use the stop indicator for circular or indeterminate progress.
- Begin low progress with a visible dot.
- Circular sizes range from 24 to 240dp.
- Linear indicators span their element's width, with at least 4dp end padding by default.
- Do not place linear indicators in elements smaller than 40dp.
- Scale waveform proportions when changing size.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/progress-indicators/accessibility).

- Give the active indicator at least 3:1 contrast against its background.
- Keep the end of a determinate linear track identifiable.
- Remove the stop indicator only when surrounding surfaces and containers provide at least 3:1 track contrast.
- Use the progress-bar accessibility role.
- Label the process and affected content.
- Describe the kind and amount of progress communicated.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
