---
name: m3-components-app-bars
description: Design, implement, test, or verify Material 3 page headlines, navigation controls, search app bars, flexible app bars, and scroll behavior.
---

# App bars

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/app-bars/overview).

Use app bars for page context, navigation, and one or two essential actions.
Choose search, small, medium flexible, or large flexible variants.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/app-bars/guidelines).

- Use a toolbar when a page has many actions.
- Emphasize only one trailing action with a filled or tonal icon button.
- Use a search app bar when global search is central to the product.
- Include Search in its hint. Selecting search opens the search view.
- Keep the container full-width with straight corners and its default height.
- Use the leading button for navigation, such as Back or Menu.
- Keep headlines concise and untruncated.
- Flexible headlines can wrap to two lines. Small headlines should not wrap.
- Place the most-used trailing actions first.
- Search app bars support up to two trailing icons on mobile and four on larger screens.
- Use fill color to separate the bar from content during scrolling.
- Flexible bars can collapse into small bars until the page returns to its top.
- Do not transform app bars into search app bars.
- Mirror leading and trailing elements for RTL languages.

## Implement the specs

Source: [Specs](https://m3.material.io/components/app-bars/specs).

- Replace baseline medium and large bars with medium flexible and large flexible bars.
- Use current common and size-specific app-bar tokens.
- Use search-component tokens for search app bars.
- Use surface at rest and surface container on scroll.
- Use body large for search, title large for small, headline medium for medium flexible, and display small for large flexible.
- Subtitle styles are label medium, label large, and title medium for small through large flexible.
- Search width fills available space until 312dp, then grows to 50% of that space.
- For transparent scrolling containers, give icon buttons filled containers.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/app-bars/accessibility).

- Maintain access to actions when content scrolls.
- Provide touch ripple, hover feedback, and visible focus indicators.
- Start focus on the leading button.
- Use Tab between interactive elements and Space or Enter to activate them.
- Prefer surface container and on surface variant for search.
- On darker backgrounds, surface bright can improve search-container contrast.
- If custom roles are necessary, maintain at least 3:1 search-text contrast against its container.
- Match the title's accessibility label to its visible text. Add page context if needed.
- Label icon buttons by their actions.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
