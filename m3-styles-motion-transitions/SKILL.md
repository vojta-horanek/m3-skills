---
name: m3-styles-motion-transitions
description: Choose and verify Material 3 transition patterns, reduced motion, stable loading layouts, and clean fades.
---

# Transitions

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read the [source manifest](../m3-styles-sources.json) for source coverage.
Open the supplied source pages for tables, diagrams, and token modules.

Source: [Transitions: Transition patterns](https://m3.material.io/styles/motion/transitions).

Source: [Transitions: Applying transitions](https://m3.material.io/styles/motion/transitions/applying-transitions).

## Select the transition pattern

- Use the legacy easing and duration system for transitions described in these sources.
- Use container transform for hero moments, shallow detail expansion, and a strong connection between elements.
- Keep a container or important hero element persistent through a container transform.
- Avoid frequent container transforms in deep, utilitarian hierarchies.
- Use platform-default forward and backward transitions for consecutive hierarchy levels.
- Use lateral transitions for peer content such as tabs, carousels, and image galleries.
- Move lateral content together without fade or parallax.
- Use a quick fade for top-level destinations in navigation bars, rails, and drawers.
- Do not use lateral motion for top-level or hierarchical navigation.
- Use enter and exit for contextual components, including dialogs, menus, sheets, and snackbars.
- Do not use enter and exit for hierarchical screen navigation.

## Apply enter and exit behavior

- On Android, expand or collapse components along x or y rather than implying z-axis elevation changes.
- Within screen bounds, iOS components scale to enter and fade to exit.
- Beyond screen bounds, iOS components slide without shape changes.
- Expand components away from the nearest screen edge.
- Keep entry locations consistent with the app's spatial model.
- When a coplanar side sheet enters, reduce the available content area.

## Keep transitions clear

- Apply transition patterns consistently.
- Keep motion grouped along a primary axis.
- Keep only important elements persistent instead of animating many independently.
- Preserve a coherent spatial model between collapsed and expanded content.
- Fully fade old content before fading new content in.
- If crossfading is necessary, keep it brief and hide it during the fastest motion.
- Do not fade a bottom sheet while it enters or exits.
- Keep common transitions simple. Avoid overt bounce effects.
- Avoid jump cuts by default. Consider them only when pure efficiency is the priority.

## Support loading and reduced motion

- Use skeleton loaders to reserve content positions and prevent layout shifts.
- Give skeletons a subtle pulse moving from top left to bottom right.
- Fade loaded content in quickly over its skeleton.
- When reduced animation is enabled, replace intense slide or scale motion with subtle fades.
- Disable decorative parallax and shape morphing under reduced animation.

## Verify

Check hierarchy cues, direction, fade overlap, loading stability, platform behavior, and reduced animation settings.
