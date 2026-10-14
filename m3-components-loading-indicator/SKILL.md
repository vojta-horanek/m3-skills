---
name: m3-components-loading-indicator
description: Design, implement, test, or verify Material 3 short indeterminate waits, contained loading, pull-to-refresh, sizing, contrast, and refresh alternatives.
---

# Loading indicators

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/loading-indicator/overview).

Use loading indicators for short processes with unknown progress. They must represent ongoing work, never decoration.
They replace most indeterminate circular indicators in Material 3 Expressive.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/loading-indicator/guidelines).

- Under 200ms, show content without an indicator.
- Between 200ms and 5s, use a loading indicator.
- Over 5s, use a progress indicator.
- Do not transition a loading indicator into a determinate progress indicator.
- Use indeterminate progress when the process can later become determinate.
- Center loading feedback in the affected page or container.
- For additional items, use their future space without covering existing content.
- Use a container when the indicator overlays content or supports pull-to-refresh.
- Pull-to-refresh applies to Jetpack Compose only.
- Use it for frequently updated content at the beginning of lists, grids, or card collections.
- Require the gesture to pass its threshold before refreshing.
- Reversing through the threshold cancels the refresh.
- Keep refresh feedback visible until completion or departure from the content.

## Implement the specs

Source: [Specs](https://m3.material.io/components/loading-indicator/specs).

- Default size is 48dp, with a 38dp shape container.
- Allow sizes from 24 to 240dp while preserving container-to-indicator proportions.
- Reserve very large indicators for large or extra-large windows.
- Use primary for an uncontained indicator.
- Use primary container with on primary container for contained loading.
- Use the seven-shape looping morph sequence.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/loading-indicator/accessibility).

- Provide at least 3:1 active-indicator contrast against its background or containing component.
- The container itself has no 3:1 requirement.
- Offer a single-pointer refresh action, such as a menu or app-bar button.
- Do not require swiping as the only refresh method.
- Use the progress-bar accessibility role.
- Label the process and affected content, such as Refreshing page.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
