---
name: m3-styles-motion-easing-duration
description: Apply or verify Material 3 legacy easing, durations, transition defaults, and platform fallback curves.
---

# Legacy easing and duration

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read [source details](references/source-map.md) for section links, source tables, diagrams, and token modules.

Source: [Easing and duration: Applying easing and duration](https://m3.material.io/styles/motion/easing-and-duration).

Source: [Easing and duration: Tokens & specs](https://m3.material.io/styles/motion/easing-and-duration/tokens-specs).

## Select the applicable system

- Migrate component motion to the spring system when adopting M3 Expressive.
- Use legacy easing and duration for transitions or products that have not yet migrated.
- Treat this legacy system as unmaintained.

## Choose easing and duration

| Movement | Emphasized default | Standard default |
| --- | --- | --- |
| Begins and ends on screen | Emphasized, 500ms | Standard, 300ms |
| Enters the screen | Emphasized decelerate, 400ms | Standard decelerate, 250ms |
| Exits permanently | Emphasized accelerate, 200ms | Standard accelerate, 200ms |

- Use emphasized easing for most transitions.
- Use standard easing for small utility transitions or unsupported emphasized platforms.
- Use emphasized easing for temporary exits so the element appears retrievable.
- Use longer durations for large transition areas and shorter durations for small areas.
- Make exits, dismissals, and collapses faster than entries and persistent motion.
- Avoid durations so short that motion becomes jarring or so long that users wait.
- Reserve durations above 600ms mainly for ambient transitions without user input.

## Implement tokens

- Use the source's exact easing and duration tokens.
- Use Standard as the CSS and iOS fallback for the full emphasized curve.
- Do not replace the full emphasized path with an invented single cubic curve.
- Read the source map for platform curves and the complete duration table.

## Verify

Check movement type, area, platform fallback, and duration against the supplied defaults and token tables.
