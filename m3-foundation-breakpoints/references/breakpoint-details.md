# Breakpoint details

## Compact

Source: [Compact](https://m3.material.io/foundations/layout/breakpoints/compact).

- Use one pane below 600dp.
- Use a navigation bar or modal expanded navigation rail.
- Put navigation near reachable window edges, such as the bottom.
- Use 16dp leading and trailing margins.
- Adapt to larger layouts when the window grows, a foldable opens, the device rotates, or split-screen ends.

## Medium

Source: [Medium](https://m3.material.io/foundations/layout/breakpoints/medium).

- Use 600–839dp for medium layouts.
- Prefer one pane because width is limited.
- Use two panes only for lower-density content with clear actions, such as settings.
- In a two-pane layout, use equal halves by default. Avoid custom widths.
- A drag handle can expand or collapse a pane to full width.
- For one pane, use a navigation rail. For two panes, use a navigation bar to preserve horizontal space.
- A secondary destination can hide its rail if a back button still reaches the primary destination.
- Use 24dp margins and a 24dp spacer between panes.
- On horizontal tablets and unfolded foldables, limit interactions in the upper 25%, which can be hard to reach.
- Avoid essential interactions too close to the bottom edge, which can also be difficult for some users.
- Consider comfortable and difficult reach regions, not only screen size.

## Expanded

Source: [Expanded](https://m3.material.io/foundations/layout/breakpoints/expanded).

- Use 840–1199dp for expanded layouts.
- Usually use two panes. A single pane can suit dense content or video.
- Use a collapsed or expanded navigation rail near the window edge.
- A secondary destination can hide its rail if back navigation still reaches the primary destination.
- Keep sorting, filtering, and secondary navigation within the pane, using tabs or other suitable controls.
- In fixed-and-flexible layouts, use a default fixed width of 360dp.
- In split-pane layouts, center the spacer visually. Navigation plus the first pane occupies half the window.
- Use 24dp leading and trailing margins and a 24dp pane spacer.

## Large and extra-large

Source: [Large and extra-large](https://m3.material.io/foundations/layout/breakpoints/large-extra-large).

- Large spans 1200–1599dp. Extra-large begins at 1600dp.
- Decide whether these sizes apply to the platform and users.
- Usually use two panes. Dense content and media can use one.
- Use a collapsed or expanded navigation rail according to content and available space.
- Expanded navigation rails suit extra-large windows. Collapse them when content needs space or navigation goes deeper.
- Keep sorting, filtering, and secondary navigation within the pane.
- In fixed-and-flexible layouts, use a default fixed width of 412dp.
- In split-pane layouts, keep the spacer visually centered, including with expanded navigation.
- Extra-large can use a standard side sheet as a third pane. Do not exceed three panes.
- A third pane can leave navigation visible, collapsed, or hidden.
- Side sheets have a default maximum width of 400dp, distinct from the 412dp fixed-pane recommendation.
- Use 24dp leading and trailing margins and a 24dp pane spacer.
- Check readability and line length as the window grows.

Every size must adapt when available space changes through window resizing, folding, orientation, or multi-window modes.
