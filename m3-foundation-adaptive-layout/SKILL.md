---
name: m3-foundation-adaptive-layout
description: Design, implement, or review Material 3 adaptive layout structure across window sizes, device contexts, preferences, and input methods.
---

# Adaptive layout

## Layout direction

Source: [Layout overview](https://m3.material.io/foundations/layout/layout-overview/overview).

- Arrange elements to show hierarchy and emphasize key actions.
- Start from an established canonical layout example.
- Use consistent arrangement, sizing, and spacing.
- Adapt across compact, medium, expanded, large, and extra-large breakpoints.
- Support both LTR and RTL languages.
- The guidance applies to Android and web.

## Building blocks

Source: [Parts of layout](https://m3.material.io/foundations/layout/layout-overview/parts-of-layout).

- Treat the window as the app's frame. Account for multi-window views and freely resized desktop windows.
- Use grids to organize related content, spacing, primary actions, and aligned bars, rails, and panes.
- Use bars to frame content and contain app or navigation bars across one or multiple panes.
- Use rails around panes for navigation, tools, chat input, FABs, and primary controls.
- Put all content in panes. Layouts have one to three panes.
- Use implicit grouping through proximity and shared background, or explicit grouping through distinct colors and outlines.
- For spatial panes, use container colors to distinguish content from the environment.
- Use drag handles to resize flexible panes or collapse and expand fixed panes.
- Use rulers as global alignment lines across layout layers.

## Context and adaptation

Source: [Adaptive design](https://m3.material.io/foundations/layout/layout-overview/adaptive-design).

- Adapt to preferences, settings, device type, orientation, resizing, and device changes.
- Consider mobile, desktop, and spatial experiences. Start with mobile and allow the design to scale to larger contexts.
- Design for touch, pointer, and physical keyboard across device categories.
- Account for mobile full-screen, split-screen, and bubble windows.
- Account for desktop free-form windows, including mobile devices connected to external displays.
- Treat panes as destinations that can resize, enter, exit, and reorganize.
- Use show/hide, levitate, or reflow strategies to adapt pane layouts.
- Adapt components through resizing, selective disclosure, or presentation changes.
- Resize components based on their content and container.
- Reveal more information when space allows, rather than only enlarging the same content.
- Change orientation, styling, or configuration when it supports the context, such as FAB to extended FAB.

## Verify adaptation

Check layout changes during resizing, orientation changes, multi-window use, and device changes.
Check that hierarchy and navigation remain understandable across those contexts.
