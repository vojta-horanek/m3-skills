---
name: m3-components-bottom-sheets
description: Design, implement, test, or verify Material 3 standard and modal bottom sheets, supplementary content, preset heights, dismissal, and accessible resizing.
---

# Bottom sheets

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/bottom-sheets/overview).

Use bottom sheets for secondary content in compact and medium windows.
Standard sheets permit interaction with main content. Modal sheets block it until an action or dismissal.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/bottom-sheets/guidelines).

- Use standard sheets for complementary content, such as audio controls.
- Use modal sheets as mobile alternatives to inline menus or simple dialogs with long action lists.
- Initially cap a modal sheet at 50% of screen height.
- Let longer content expand to full-screen height and scroll internally.
- Show a close affordance in full-screen modal sheets.
- Allow modal dismissal through an action, scrim, downward swipe, or available close control.
- Full-screen standard sheets need a collapse control.
- Selectable drag handles must cycle preset heights and permit closing without dragging.
- If there is no drag handle, provide another single-pointer resize action.
- Scrim selection closes the modal sheet.
- Consider side sheets for expanded desktop layouts.
- Keep overflowing sheet content accessible through scrolling.

## Implement the specs

Source: [Specs](https://m3.material.io/components/bottom-sheets/specs).

- Use surface container low, on surface variant for the handle, and a scrim for modal sheets.
- On Android, system UI handles scrim color and opacity.
- Use 28dp top corner radii.
- Span the window width up to 640dp.
- Use 72dp top margin in the default measurement configuration.
- For windows wider than 640dp, use 56dp top and side margins.
- Center the drag handle with 22dp vertical padding.
- Height is variable.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/bottom-sheets/accessibility).

- Reserve the top 48dp as an interactive region when the drag handle supports resizing.
- Include the handle in tab order for keyboard and switch input.
- Give the drag handle a button role and accessibility label.
- Tab reaches the handle. Space or Enter cycles available heights.
- Provide a single-pointer alternative for every drag action.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
