---
name: m3-foundation-text-adaptation
description: Design, implement, or verify Material 3 text wrapping, truncation, 200 percent resizing, reflow, scrolling, and enlarged tooltips.
---

# Text adaptation

## Truncation and wrapping

Source: [Text truncation](https://m3.material.io/foundations/writing/text-truncation).

- Preserve content, comprehension, and functionality when text size, spacing, translation length, viewport, or zoom changes.
- The source notes that exceptions may apply to non-Latin alphabet languages.
- Wrap critical text, text needed for understanding, and text when space permits.
- If wrapped text still does not fit, provide a way to reveal the rest.
- Allow containers to extend vertically or horizontally to fit their content.
- Do not impose limits that waste available space.
- Use ellipses only when a tooltip or link makes the omitted text available.
- A link within truncated content must reveal that omitted content.
- Ellipses without access to the full text are inaccessible. Revealing truncated text can still add difficulty for some users.

## Resizing

Source: [Text resizing](https://m3.material.io/foundations/writing/text-resizing).

- Support a text increase of at least 200%.
- Scale text and line height proportionally with the scale value.
- Keep component padding and internal spacing at their default 1× values for most components.
- Do not scale components without text, such as checkboxes, radio buttons, and progress indicators, for text resizing.
- If the OS does not control resizing, offer multipliers such as 1.5× and 2×.
- Calculate scaled font size as the default font size multiplied by the scale value.
- Increase container size to prevent overlap, clipping, or unwanted truncation.
- Reflow long components. Stack them instead of fixing them side by side when necessary.
- Let long content scroll. Prefer vertical scrolling and avoid requiring scrolling in both directions.
- For top app bars, navigation bars, navigation rails, and fixed top tabs, touch-and-hold tooltips can show enlarged labels.
- In that constrained-space method, keep the component label at 1× and show its enlarged version in the tooltip.

## Verify adaptation

Check at 200% text size and with longer text or increased spacing.
Check for clipping, overlap, unwanted truncation, missing content, and inaccessible enlarged labels.
Check that scaling affects text and line height without also scaling default padding or text-free controls.
