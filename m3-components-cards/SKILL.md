---
name: m3-components-cards
description: Design, implement, test, or verify Material 3 single-topic cards, collections, action surfaces, responsive layouts, gestures, and focus.
---

# Cards

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/cards/overview).

Use cards to contain related content and actions on one topic.
Choose elevated, filled, or outlined cards. Content determines their layout and dimensions.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/cards/guidelines).

- Use clear text and image hierarchy so cards are easy to scan.
- Do not force content into cards when spacing, headings, or dividers would be simpler.
- Keep collection cards at the same resting elevation.
- Place collection filtering and sorting controls outside the collection.
- Apply a collection filter to every card.
- Avoid text on images. If necessary, use sufficient contrast with a scrim or bounding shape.
- On mobile, expand cards to reveal content. Do not scroll content inside a card.
- Desktop cards can contain expanded, scrollable content.
- Assign only one swipe action per card.
- Do not combine card swipes with swipeable content inside that card.
- Raise a card's elevation when moving it. Do not displace other elements.
- Adapt spacing and orientation for larger windows.
- Consider columns or carousels on large screens and lists on small screens.
- Preserve controls and actions when changing components.

## Implement the specs

Source: [Specs](https://m3.material.io/components/cards/specs).

- Use a 12dp container corner radius.
- Use 16dp horizontal padding and a maximum 8dp gap between cards.
- Start-align label text.
- Use surface container low for elevated cards.
- Use surface container highest for filled cards.
- Use surface and outline variant for outlined cards.
- Implement hovered, focused, pressed, dragged, and disabled states for actionable cards.
- A container is required. Other card elements are optional.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/cards/accessibility).

- Choose a directly actionable card without nested actions, or a non-actionable card with internal actions.
- Do not place an action on an actionable surface.
- Provide a single-pointer alternative for dragging or swiping, such as menu actions.
- Ensure any menu used during dragging remains usable.
- Directly actionable cards receive ripple, hover, and focus feedback.
- Make directly actionable cards tab stops with button or link roles as appropriate.
- Non-actionable containers need no role or tab stop.
- Give every internal action a tab stop before focus leaves for the next card.
- Support Space or Enter activation.
- Announce informative content and hide decorative images from screen readers.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
