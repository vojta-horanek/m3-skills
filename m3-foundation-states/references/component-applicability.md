# State applicability

Source: [Applying states](https://m3.material.io/foundations/interaction/states/applying-states).

The source lists these component groups. Some examples and lists differ, as noted below.

| State | Listed as inheriting | Listed as not inheriting |
| --- | --- | --- |
| Disabled | Buttons, cards, checkboxes, chips, list items, radio buttons, switches, text fields | App bars, badges, dialogs, FABs, menus, navigation bars/drawers/rails, sheets, tabs, tooltips |
| Hover | Buttons, cards, checkboxes, chips, date/time pickers, list items, sliders, switches, text fields | App bars, badges, dialogs, menus, navigation bars/drawers/rails, sheets, tabs |
| Focused | Buttons, cards, checkboxes, chips, date/time pickers, list items, selection controls, text fields | App bars, badges, banners, cards, dialogs, navigation bars/drawers/rails, sheets |
| Pressed | Buttons, cards, checkboxes, chips, list items, text fields | App bars, badges, bottom navigation, dialogs, menus, sheets, tabs |
| Dragged | Cards, chips, list items, sliders | App bars, badges, buttons, dialogs, menus, navigation bars/drawers/rails |

Cards appear in both focused-state lists. The page does not resolve that conflict.
The focus and press sections also say these states apply to all interactive components.
Examples show FAB hover and focus even though FABs are not named separately in those inclusion lists.
Keep these distinctions visible when using the source. The lists do not establish an invented universal rule for ambiguous cases.

For composite containers, the explicit guidance applies states to actionable child components rather than the whole container.
