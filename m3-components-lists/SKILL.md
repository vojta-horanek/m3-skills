---
name: m3-components-lists
description: Design, implement, test, or verify Material 3 scannable list items, selection modes, flexible slots, adaptive content, swipe alternatives, and focus.
---

# Lists

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/lists/overview).

Use lists to help people find and act on discrete items.
Prefer expressive lists for new designs. Standard and segmented styles do not change behavior.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/lists/guidelines).

- Keep labels, supporting visuals, and actions in consistent positions.
- Keep supporting text to one to three lines.
- Use leading visuals as scanning anchors and trailing elements for supplementary details or actions.
- Choose one mode at a time: single-action, multi-action, single-select, or multi-select.
- Single-action items cannot have secondary nested actions or persistent selection.
- Single-select items use radio buttons without nested actions.
- Multi-select items use checkboxes or switches without nested actions.
- Multi-action items give the primary action most space and secondary actions the trailing position.
- Use one selection interaction per item.
- Prefer gaps for contained lists and dividers only when stronger separation is needed.
- Adapt margins, content, or columns to keep text readable on larger screens.
- Use full-screen details in compact windows and side-by-side list-detail layouts in larger windows.
- Swipe-to-reveal is available only on Android Views.

## Implement the specs

Source: [Specs](https://m3.material.io/components/lists/specs).

- Require a container and label. Other elements are optional.
- Keep content slots wider than leading and trailing slots.
- Preserve standard padding and targets of at least 48×48dp in custom slots.
- Unselected expressive corners are 4dp internally and 16dp externally.
- Selected corners are 16dp throughout.
- Baseline item heights are 56, 72, or 88dp, determined by the tallest element.
- Baseline elements are normally middle-aligned, but top-aligned at 88dp or with three text lines.
- Use the current common and expand token sets.
- Include selected and unselected interaction states.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/lists/accessibility).

- Show selection through two cues, such as color and a checkmark.
- Provide single-pointer alternatives to hidden swipe actions.
- Single-action entry focuses the selected item, or the first item if none is selected.
- Multi-action entry focuses the first internal action. The whole item is not selectable.
- Arrows navigate items or internal actions. Space or Enter activates them.
- Down or Right advances. Up or Left goes backward. Wrap at list endpoints.
- Label items with visible label and supporting text.
- On web, selectable containers use List box and items use Option with selected states.
- On Android, single-select items use radio semantics and multi-select items use checkbox semantics.
- Label nested controls according to their platform guidance.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
