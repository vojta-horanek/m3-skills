---
name: m3-styles-shape-morph
description: Apply or verify Material 3 shape morphs for interaction states, progress, and environmental changes.
---

# Shape morph

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read the [source manifest](../m3-styles-sources.json) for source coverage.
Open the supplied source pages for tables, diagrams, and token modules.

Source: [Shape: Shape morph](https://m3.material.io/styles/shape/shape-morph).

Source: [Shape: Overview & principles](https://m3.material.io/styles/shape).

## Apply morphs

- Use Material shape morphs to clarify interactions and communicate change.
- Use morphs for selected states, actions in progress, or environmental changes.
- Match morph responses to interactions such as taps, swipes, scrolls, release, and long presses.
- Use the platform-specific Material shape library API.
- On Android, use the Shapes in Compose API.
- Do not assume Web support. The supplied source lists Web as unavailable.
- Use the expressive motion scheme by default. Switch to standard when needed.
- Recognize standard button groups and loading indicators as supplied morph examples.

## Verify

Check that each morph supports comprehension without compromising clarity.
Check the intended interaction or progress state and the applicable motion scheme.
For reduced animation behavior, use the supplied transition accessibility guidance.
