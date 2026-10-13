---
name: m3-foundation-canonical-layouts
description: Choose, implement, or verify Material 3 feed, list-detail, and supporting-pane layouts and their adaptive navigation and persistent state.
---

# Canonical layouts

## Choose the content relationship

Source: [Canonical examples overview](https://m3.material.io/foundations/layout/canonical-examples/overview).

- Use canonical examples as starting points for the layout scaffold.
- Use a feed for browsing many content items in a configurable grid.
- Use list-detail for a list and the details of its items.
- Use supporting panes for secondary content meaningful only in relation to primary content.
- For custom layouts, build on canonical examples or layer scaffold elements.
- Use levitated panes for focused temporary tasks, such as a shopping basket or event creation.

## Feed

Source: [Feed](https://m3.material.io/foundations/layout/canonical-examples/feed).

- Use cards and lists for browsing and discovery.
- Let content vary in proportions and size. Use size and position to express relationships.
- Reflow items when available space changes. Item position determines their order.
- At compact widths, stack items vertically so each fills the pane width.
- At medium widths, use multiple columns and different component widths when appropriate.
- At expanded and larger widths, usually increase the number of columns. Columns can also grow wider.

## List-detail

Source: [List-detail](https://m3.material.io/foundations/layout/canonical-examples/list-detail).

- Use one visible view at compact widths, showing either list or detail.
- At medium widths, prefer one pane for dense content or deep focus.
- Medium two-pane layouts can suit collection browsing and quick item switching.
- Use bottom navigation or a modal rail to preserve width in medium two-pane layouts.
- At expanded and larger widths, show both panes.
- Show the detail back button only in a single-pane layout.
- Show the selected list item state only in a two-pane layout.
- Use grouping to direct visual focus in two-pane layouts.
- With no selection, show the list in a single pane and placeholder detail content in two panes.
- With a selected item, expanding to two panes shows its details alongside the list.
- When shrinking, normally show the detail with an app bar.
- For selection without deep navigation, such as multi-select, retaining the list can be appropriate.
- Keep transitions consistent with the view previously shown. Multi-select can retain the most recently used pane.
- Preserve detail state between items, including scroll position and read or unread status.

## Supporting pane

Source: [Supporting pane](https://m3.material.io/foundations/layout/canonical-examples/supporting-pane).

- Give primary content most of the space, typically about two-thirds.
- Use the remainder for content that supports the primary area.
- For parent-child content, use list-detail instead.
- At compact and medium widths, place supporting content below the primary pane with flexible width.
- At compact widths, a bottom sheet can provide supporting content while retaining primary focus.
- At expanded widths, place the supporting pane on the leading or trailing side, with a fixed width of 360dp.

## Verify the chosen pattern

Check content relationships, visible views, item order, back navigation, selection indicators, and persistent detail state across size changes.
