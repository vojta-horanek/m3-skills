---
name: m3-styles-motion-springs
description: Implement and verify Material 3 physics motion schemes, spatial springs, effects springs, and platform conversions.
---

# Spring motion

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read [source details](references/source-map.md) for section links, source tables, diagrams, and token modules.

Source: [Motion physics system: How it works](https://m3.material.io/styles/motion/overview).

Source: [Motion physics system: Specs](https://m3.material.io/styles/motion/overview/specs).

## Choose a scheme

- Use the physics motion system for components and new motion implementations.
- Use expressive motion for most situations, especially hero moments and key interactions.
- Use standard motion for utilitarian products requiring minimal bounce.
- Keep most product motion within the same scheme.
- Override the scheme selectively to emphasize key moments.
- Set the scheme at product level. Do not add its name to individual spring token names.

## Assign springs

- Use spatial springs for position, rotation, size, and corner changes.
- Use effects springs for color and opacity without overshoot.
- Use default speed for most motion and partial-screen animations.
- Use fast speed for small elements such as switches and buttons.
- Use slow speed for full-screen motion or content refresh.
- For example, use md.sys.motion.spring.fast.spatial within the selected scheme.
- Treat stiffness, damping, and initial velocity as the spring's behavioral attributes.

## Apply by platform

- On Jetpack Compose, use built-in components and spring tokens.
- For custom Compose schemes, return the required AnimationSpec values from a MotionScheme object.
- Override CompositionLocal to change the scheme for a specific composable, screen, or element.
- On Android Views, use built-in spring tokens. Do not assume components already apply them.
- On Web, use springs where possible.
- Use the source conversion curves only for animations without gestures or interruptions.
- Read the source map for exact spring-to-curve pairs.
- Keep transition-specific legacy guidance separate from component spring motion.

## Verify

Check scheme consistency, spatial/effects assignments, speed choice, gesture interruption, and retargeting behavior.
Check the platform context before using token values.
