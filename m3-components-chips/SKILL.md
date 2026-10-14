---
name: m3-components-chips
description: Design, implement, test, or verify Material 3 assist, filter, input, and suggestion chips, sets, secondary actions, overflow, and semantics.
---

# Chips

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/chips/overview).

Use chip sets for contextual actions, filtering, or discrete information.
Assist chips represent actions. Filter chips narrow collections. Input chips are user-authored. Suggestion chips are product-authored.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/chips/guidelines).

- Use buttons for major actions and task progression. Do not substitute chips for these actions.
- Show chips in sets, not alone.
- Keep labels within 20 characters where possible.
- Start assist labels with verbs. Use category nouns for filters and short phrases for suggestions.
- Use one selection behavior across the page's filter sets, either single-select or multi-select.
- Show a leading checkmark when a filter is selected.
- Input chips can return to text for editing.
- Keep a removal action on removable input chips, subject to the mobile-only remove-action exception.
- Separate primary and secondary targets so they do not interfere.
- Use at least 8dp between chips.
- Wrap or horizontally scroll sets as needed.
- After more than two filter rows, consider horizontal scrolling.
- Keep outlines on plain backgrounds. Elevate only when visual separation requires it.
- Use ripple feedback rather than elevation for pressing.

## Implement the specs

Source: [Specs](https://m3.material.io/components/chips/specs).

- Use 32dp visible container heights with 8dp corner radii and 18dp icons.
- Use 8dp between internal elements.
- Assist, filter, and suggestion chips use 16dp horizontal padding without icons and 8dp with icons.
- Input avatars measure 24dp with 12dp corner radii.
- Input avatar padding is 4dp leading and 8dp trailing.
- Give removal icons targets of at least 48dp.
- For two actions, use at least 88dp container width or 42dp label width.
- Apply the current variant-specific color and state tokens.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/chips/accessibility).

- Maintain 48dp chip targets and at least 3:1 label contrast.
- Do not apply density by default. Keep density-reversal controls at 48×48 CSS pixels.
- Provide a way to expose all horizontally overflowed chips without scrolling.
- Use a leading Show all filter to reflow, or a button to open a menu.
- Do not use that menu method for chips with secondary actions.
- Tab focuses enabled chips or groups. Arrows move between chips.
- Space or Enter activates or toggles. Backspace or Delete removes a focused input chip.
- Label chips with their text and removal actions separately.
- A two-action chip has two focusable elements. A remove-only chip is one focusable element.
- Hide decorative chip images from assistive technology.
- Web basic and selectable chips use Gridcell roles. Android basic chips use Button roles.
- Selectable Android Views chips use Radio button roles. Selectable Compose chips use Checkbox roles.
- Two-action chips use Button or Checkbox roles according to their action.
- Show interactivity through group instructions, page context, a 3:1 outline, an action label, or a leading icon.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
