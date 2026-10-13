---
name: m3-foundation-scaffold
description: Design, implement, or verify Material 3 bars, rails, panes, safety regions, pane resizing, and pane focus behavior.
---

# Layout scaffold

## Regions

Source: [Scaffold overview](https://m3.material.io/foundations/layout/scaffold/overview).

Organize adaptive layouts into bars, rails, and panes.
Bars frame navigation, rails surround panes with controls, and panes contain primary content.

## Bars

Source: [Bars](https://m3.material.io/foundations/layout/scaffold/bars).

- Let bars span a single pane or the full window.
- Put app bars at the top with a title and one or two essential actions.
- Use navigation bars for three to five primary views at compact or medium breakpoints.
- Place bars beside system safety regions. Do not put primary content inside those regions.

## Rails

Source: [Rails](https://m3.material.io/foundations/layout/scaffold/rails).

- Use top and bottom rail regions on compact screens for tools, chat input, FABs, and primary screen controls.
- On larger screens, use the leading side rail region for navigation.
- Use the trailing rail region for controls that support or modify pane content.
- Rails can surround panes or float above them.
- In XR, rail components can become orbiters outside the main content area.

## Panes

Source: [Panes](https://m3.material.io/foundations/layout/scaffold/panes).

- Use one to three visible panes. Include at least one flexible pane.
- Use a single flexible pane at compact and usually medium breakpoints.
- Prefer two panes at expanded, large, and extra-large breakpoints. Extra-large can also support three.
- A split-pane layout keeps the spacer visually centered.
- With a side navigation region, navigation plus its adjacent pane occupies half the window. The other pane retains half.
- With bottom navigation or no navigation, both panes use half the width by default.
- A fixed-and-flexible layout can place the fixed pane on either side according to the content.
- At extra-large widths, a standard side sheet can form a third pane. Its default maximum width is 400dp.
- For expanded, large, and extra-large resizing, recommended snap widths are 360dp, 412dp, or a visually centered split.
- Let a drag handle resize panes and also toggle sizes through selection, such as tap, double tap, or long press.
- Use persistent resizing for most resizable layouts. Preserve widths across app closure and breakpoint changes, including a collapsed pane.
- Use temporary resizing mainly for supporting panes with uncommon resizing. Restore defaults after the pane or product closes and reopens.

## Presentation and focus

- Keep persistent utilities co-planar with primary content for accessibility.
- Keep temporary tasks floating across breakpoints, such as dialogs.
- Dock supplementary panes to a window edge when appropriate.
- Adapt panes by showing/hiding, levitating, or reflowing. Preserve context and meaning.
- Provide accessible controls for moving or resizing floating panes.
- On large screens, floating panes are the default and their scrim is optional.
- Docked panes can become floating or co-planar at medium and expanded sizes. Consider co-planar presentation on large screens.
- Reflow panes vertically when horizontal space is insufficient.
- In XR, distinguish spatial panels clearly from their background.
- For co-planar and docked panes, match focus order to visual arrangement.
- For a modal pane, prevent interaction with background elements and move focus to its first element.
- On closing a modal pane, return focus to its trigger. For an automatic trigger, use the next logical element.
- The source says a modal floating pane disappears on interaction behind it, while background elements remain inoperable.
- For a non-modal pane, permit interaction elsewhere and focus movement into and out of the pane.
- Put non-modal panes in logical reading order. Docked panes follow the corresponding modal or non-modal focus requirements.

## Verify the scaffold

Check safety regions, pane count, flexible sizing, centered splits, resizing persistence, and focus behavior.
