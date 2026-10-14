---
name: m3-styles-color-user-generated
description: Design and verify Material 3 dynamic color sourced from an Android user wallpaper.
---

# User-generated dynamic color

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read the [source manifest](../m3-styles-sources.json) for source coverage.
Open the supplied source pages for tables, diagrams, and token modules.

Source: [Dynamic: User-generated source](https://m3.material.io/styles/color/dynamic/user-generated-source).

## Apply wallpaper-based roles

- Let the system analyze wallpaper, select a source color, and assign tones to roles.
- Design with color roles rather than particular hex values.
- Use Material Theme Builder to generate a working scheme.
- Enable New theme color diagram and Generate State Layers.
- Create and name a theme, then set a Primary source color.
- Select the theme and relevant frames, then select Swap for M3 kit components.
- Copy the scheme diagram into existing files to expose its local styles.
- Replace remaining direct values and unrelated styles with roles matching their use.

## Verify potential schemes

1. Open Material Theme Builder.
2. Select Dynamic.
3. Add an image or select Shuffle for a random source color.
4. Select the frames or components under review.
5. Select Swap.
6. Repeat across a range of colors to examine different users' potential results.

Use the development link in the source page for Android Views integration.
