---
name: m3-foundation-accessibility-elements
description: Label Material 3 controls and meaningful visuals, assign semantic roles, and hide decorative elements for assistive technology.
---

# Accessible elements

Source: [Elements](https://m3.material.io/foundations/designing/elements).

## Decide what needs a label

- Label interactive icons or buttons without sufficient visible text or context.
- Label interactive images, meaningful images, meaningful status icons, progress cues, and error cues.
- Add context to generic links and buttons when their purpose is ambiguous.
- Do not add redundant labels to ordinary non-interactive text or buttons with sufficient text.
- Mark decorative images and icons for hiding when they add nothing to the nonvisual experience.

## Write and assign labels

- Describe content, purpose, and behavior concisely.
- For action icons, describe the task rather than the icon's appearance.
- For meaningful images, describe their content and context.
- Do not include the element role, such as button or menu, in its label.
- Assign the proper role separately. Screen readers announce the role automatically.
- Translate accessibility labels into the label mechanism used by the target platform.
- For the web, assign appropriate ARIA roles to interactive elements.
- For other platforms, use the corresponding component control type.
- Define the role from intended behavior. Visually similar elements can have different interaction patterns.

## Verify elements

Check that labels explain tasks and meaning without repeating announced roles.
Check that generic actions are distinguishable and decorative elements do not interrupt reading.
