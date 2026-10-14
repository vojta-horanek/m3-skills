---
name: m3-components-search
description: Design, implement, test, or verify Material 3 search entry points, contained and docked layouts, suggestions, results, clearing, and announcements.
---

# Search

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read the [source manifest](../m3-components-sources.json) for source coverage.
Open the supplied source pages for measurement diagrams and token tables.

## Choose the component

Source: [Overview](https://m3.material.io/components/search/overview).

Use search to find information through queries.
Prefer the contained style over the divided baseline style. Suggestions and results use lists.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/search/guidelines).

- Use a search bar for a specific view.
- Use a search app bar for global search or an icon for secondary search.
- Keep the search bar near the searchable content.
- Show suggestions before entry or suggestions and results during entry as the product requires.
- Use docked focused search for medium and expanded windows.
- Use full-screen focused search for compact windows.
- Keep the contained search shape persistent.
- Use one or two trailing actions, or an avatar with one other action.
- Explain the searchable content in the hint.
- Group result lists with context such as categories, avatars, or filter chips.
- Give focused search a clear status indicator, such as a search icon or Results label.
- Enter executes a query. A suggestion or result can also be selected directly.
- Keep query text visible after search, without retaining its focus.
- Back dismisses focused results and restores the original bar.

## Implement the specs

Source: [Specs](https://m3.material.io/components/search/specs).

- Use search-bar tokens for unfocused search and search-view tokens for focused search.
- Default bar height is 56dp and its width ranges from 360 to 720dp.
- Unfocused outer margins are 24dp. Focused margins are 12dp.
- Avatars measure 30dp.
- Docked result containers range from 240dp to two-thirds of screen height.
- Full-screen result containers fill the window.
- Apply each internal element's own interaction states.
- Search's result container is empty by default. Add list content.
- Use surface container roles more than one step apart for clear separation.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/search/accessibility).

- Announce the appearance of suggestions or results through a screen reader.
- Focus the first interactive element, usually a leading control or the text field.
- Tab and Shift+Tab navigate controls.
- Space or Enter activates text input. Arrows navigate result items.
- Use the search hint as the accessibility label.
- Input roles are Text field on Android and Search field on iOS.
- Label icon buttons by their actions.
- Follow list accessibility directions for results.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
