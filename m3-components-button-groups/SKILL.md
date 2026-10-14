---
name: m3-components-button-groups
description: Design, implement, test, or verify Material 3 standard and connected button groups, selection, spacing, and focus.
---

# Button groups

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/button-groups/overview).

Use standard groups for related actions. Use connected groups for related selectable options.
Connected groups replace segmented buttons in Material 3 Expressive.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/button-groups/guidelines).

- Use the same size and shape by default within a standard group.
- Reserve mixed sizes for prominent moments and shape differences for meaningful interactions.
- Use connected groups for single-select or multi-select toggle patterns.
- Do not mix color styles in a connected group.
- Avoid text buttons and standard icon buttons without a visible container treatment.
- Let standard groups fit their contents.
- Let connected groups fill their surface. Consider a maximum width on large screens.
- Keep each group on one line. Do not wrap its buttons.
- Preserve the primary action's visual emphasis across breakpoints.
- Place overflow actions at the trailing end when space becomes limited.
- In standard groups, change the pressed button's width and shape and adjust adjacent widths.
- In connected groups, change only the selected or pressed button's shape.

## Implement the specs

Source: [Specs](https://m3.material.io/components/button-groups/specs).

- Select token sets by variant and size.
- Use standard inner padding of 18dp for XS, 12dp for S, and 8dp for M, L, and XL.
- Use 2dp inner padding for every connected-group size.
- Use connected inner corner radii of 4, 8, 8, 16, and 20dp for XS through XL.
- For square connected groups, use these radii for outer corners too.
- Keep XS and S connected buttons at least 48dp wide with 48dp target areas.
- Allow group height to follow its buttons, including their density settings.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/button-groups/accessibility).

- Give every button a target of at least 48×48dp.
- Do not reduce XS or S inner padding.
- Keep the group container outside the focus order.
- Place initial focus on the first button.
- Support Tab navigation, arrow navigation within the group, and Space or Enter activation.
- Label each button according to button or icon-button guidance.
- The container does not need an accessibility label.
- Make selected buttons identifiable through assistive technology.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
