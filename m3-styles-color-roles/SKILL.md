---
name: m3-styles-color-roles
description: Assign and verify Material 3 accent, surface, outline, inverse, error, and fixed color role pairs.
---

# Color roles

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read [source details](references/source-map.md) for section links, source tables, diagrams, and token modules.

Source: [Color roles: Tab 1](https://m3.material.io/styles/color/roles).

## Pair roles correctly

- Apply colors only in the intended pairs and layering orders.
- Use container roles for fills. Do not use them for text or icons.
- Use each on-color for text and icons on its corresponding parent color.
- Do not substitute unrelated roles because their current colors appear similar.

## Assign accent and error roles

- Use primary for prominent actions, high-emphasis elements, and active states.
- Pair primary with on primary. Pair primary container with on primary container.
- Use secondary for less prominent elements, such as filter chips and tonal buttons.
- Pair secondary with on secondary. Pair secondary container with on secondary container.
- Use tertiary for complementary accents and smaller elements needing special emphasis.
- Pair tertiary with on tertiary. Pair tertiary container with on tertiary container.
- Use error roles to communicate errors and urgency.
- Pair error with on error. Pair error container with on error container.
- Keep default error colors static under dynamic color. Allow their light and dark theme adaptation.

## Assign surfaces and inverse roles

- Use surface for default backgrounds.
- Use surface container lowest, low, default, high, and highest to express container emphasis.
- Use on surface for text and icons on any surface or surface container.
- Use on surface variant for lower-emphasis text and icons on these surfaces.
- Keep region color roles consistent across breakpoints.
- Add surface roles on larger layouts only with consistent hierarchy and application.
- For contrasting inverse areas, use inverse surface with inverse on surface.
- Use inverse primary for actionable elements against inverse surface.

## Assign outlines

- Use outline for important boundaries, such as text fields.
- Use outline variant for dividers, decorative boundaries, and multi-element containers such as cards.
- Do not use outline variant alone to define target boundaries or visual hierarchy.
- Use outline or another color with 3:1 surface contrast when a target boundary needs contrast.
- Outline variant can border targets when their internal text and icons provide 4.5:1 contrast.

## Use add-on roles only when needed

- Use fixed accent roles when fills must retain their tone across light and dark themes.
- Use fixed dim for a stronger tone with the same theme behavior.
- Pair fixed fills with their corresponding on fixed or lower-emphasis on fixed variant colors.
- Avoid fixed fills where contrast against the surrounding surface is necessary.
- Use regular primary, secondary, or tertiary roles where accent contrast is needed.
- Use surface bright or surface dim when relative brightness must persist across both themes.

## Verify

Check intended pairs across dynamic source colors, themes, and contrast settings.
Check that responsive layouts retain region mappings and that fixed roles do not impair contrast.
