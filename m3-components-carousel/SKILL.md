---
name: m3-components-carousel
description: Design, implement, test, or verify Material 3 carousel layouts, visual browsing, scrolling, accessible alternatives, and reduced motion.
---

# Carousels

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/carousel/overview).

Use carousels for visual items with brief optional text.
Layouts include multi-browse, uncontained, uncontained multi-aspect ratio, hero, center-aligned hero, and full-screen.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/carousel/guidelines).

- Use multi-browse for several simple visuals and hero for spotlighted content.
- Use uncontained layouts for more text or customization.
- Use multi-aspect ratio only when item widths vary, from 9:16 to 16:9.
- Keep large images recognizable and text readable.
- In compact windows, show at most three text-bearing multi-browse items unless their content remains clear.
- Prefer snap scrolling for multi-browse and hero layouts.
- Use default scrolling only for uncontained layouts.
- Use full-screen layouts for portrait, vertically scrolling media in compact or medium windows.
- Full-screen items must snap to container edges. Do not use them in landscape.
- On vertically scrolling pages, provide access to all items without horizontal scrolling.
- Prefer a Show all button below the carousel or an arrow beside its header.
- Do not place controls over, inside, or directly beside the carousel.

## Implement the specs

Source: [Specs](https://m3.material.io/components/carousel/specs).

- Use 28dp item corner radii except in full-screen layouts.
- Small items have dynamic widths between 40 and 56dp.
- Use 8dp item gaps and 8dp vertical padding for non-full-screen layouts.
- Use 16dp leading and trailing padding for multi-browse and hero layouts.
- Uncontained layouts use 16dp leading padding.
- Full-screen layouts have no outer padding and 16dp item gaps.
- Use enabled, hovered, focused, pressed, and disabled item states.
- Keep widths dynamic as items change position and container size.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/carousel/accessibility).

- Focus the first item, not the container.
- Support Tab or arrows between items and Space or Enter activation.
- Use up and down arrows to leave the carousel for surrounding elements.
- Label the container and expose its container role.
- Announce the current item and total item count.
- Give a header arrow a 48dp size. Give Show all 4dp padding.
- Repeat the carousel header on the all-items page.
- With reduced motion, remove parallax and item expansion.
- Make items the same size and extend the layout to the window edges to avoid clipping.
- Reduced-motion hero previews can remain partially visible.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
