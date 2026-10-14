---
name: m3-components-tabs
description: Design, implement, test, or verify Material 3 primary and secondary related content, fixed and scrollable tabs, labels, swipe behavior, and focus.
---

# Tabs

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/tabs/overview).

Use tabs for related content at the same hierarchy level.
Primary tabs show main content categories. Secondary tabs divide content within a category.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/tabs/guidelines).

- Do not use tabs for sequential content that needs a fixed reading order.
- Place primary tabs below the app bar and secondary tabs below primary tabs.
- Use a single row with a consistent label and icon treatment.
- Keep labels short. Prefer scrollable tabs over unnecessary truncation.
- Use globally recognizable icons when labels are absent.
- Do not mix icon-and-text tabs with other tab formats in the same set.
- Prefer no more than four fixed tabs. Use scrolling when more cannot fit.
- Offset the first scrollable tab by 52dp from the leading edge.
- Let scrollable widths follow labels with consistent padding.
- Show active tabs through an underline and color change.
- Update or remove tab badges after their content is viewed.
- Fixed tabs may support swiping through content.
- Avoid conflicting swipe directions in nested content.
- Move attached tabs with their component, rather than behind an app bar.

## Implement the specs

Source: [Specs](https://m3.material.io/components/tabs/specs).

- Use 48dp height for label-only tabs and 64dp for icon-and-label tabs.
- Icons measure 24dp. Dividers are 1dp inside the container.
- Primary indicators are 3dp high. Secondary indicators are 2dp high.
- Primary indicators have 2dp side insets and a minimum 24dp length.
- Use 8dp between inline icons and text and 4dp between inline text and badges.
- Stacked icon badges overlap by 6dp.
- Apply active and inactive hover, focus, and pressed states.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/tabs/accessibility).

- Support keyboard access to off-screen tabs.
- Do not make scrollable sets loop infinitely, which can trap linear screen reader navigation.
- Use Tab or arrows to navigate and Space or Enter to activate.
- Keep a visible focus indicator.
- Do not apply density by default.
- If users choose density, keep reversal targets at least 48×48 CSS pixels.
- Use descriptive labels for ambiguous or icon-only tabs.
- Maintain access to primary actions while content scrolls.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
