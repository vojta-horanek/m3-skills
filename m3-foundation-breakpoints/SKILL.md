---
name: m3-foundation-breakpoints
description: Apply and verify Material 3 compact, medium, expanded, large, and extra-large window breakpoints, pane widths, navigation, and margins.
---

# Breakpoints

## Available window space

Source: [Breakpoints overview](https://m3.material.io/foundations/layout/breakpoints/overview).

Design for available window space rather than fixed device categories.
Orientation, folding, multi-window use, and free-form resizing can change the breakpoint.
Android also provides compact, medium, and expanded height breakpoints. Vertically scrolling layouts rarely need height-based changes.

| Breakpoint | Window width | Usual pane choice |
| --- | --- | --- |
| Compact | Under 600dp | One |
| Medium | 600–839dp | One, or two for suitable low-density content |
| Expanded | 840–1199dp | Usually two |
| Large | 1200–1599dp | Usually two |
| Extra-large | At least 1600dp | Usually two, with up to three supported |

- For each size change, consider what to reveal, divide, resize, reposition, or swap.
- Reveal useful content or controls instead of simply enlarging everything.
- Preserve a single-pane experience when a focused task or dense media benefits from it.
- Adjust margins and typography to keep text around 40–60 characters per line.
- Swap only functionally equivalent components for an ergonomic or functional reason.
- Do not arbitrarily replace a button with a chip or menu. Use caution when changing lists into cards.
- Compact supplemental selection can use a bottom sheet. Medium and larger layouts can use a menu.
- Compact communication can use a basic or full-screen dialog. Larger layouts usually use a basic dialog.

## Size-specific guidance

Read [breakpoint details](references/breakpoint-details.md) for the requested sizes.
It covers every compact, medium, expanded, large, and extra-large source tab.

## Verify transitions

Check changes during rotation, folding, split-screen use, multi-window use, and free-form resizing.
Check pane count, navigation access, spacing, text line length, and functional equivalence of swapped controls.
