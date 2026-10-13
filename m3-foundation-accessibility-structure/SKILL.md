---
name: m3-foundation-accessibility-structure
description: Design, implement, or audit accessible Material 3 hierarchy, semantic structure, landmarks, headings, and interaction targets.
---

# Accessible structure

## Platform semantics

Source: [Designing overview](https://m3.material.io/foundations/designing/overview).

- Include accessibility markup in design specifications.
- Use standard platform controls and semantic HTML to support platform assistive technology.
- Follow platform accessibility standards, shortcuts, and structure.
- A non-standard element performing a standard task needs extra assistive-technology testing.

## Hierarchy and navigation

Source: [Structure](https://m3.material.io/foundations/designing/structure).

- Use visible elements, sufficient contrast and size, clear hierarchy, and key information recognizable at a glance.
- Keep task flows short and controls easy to locate and understand.
- Combine visual and textual cues, such as color, shape, text, and motion, to show importance.
- Put important actions at the top or bottom, where shortcuts can reach them.
- Put related items with similar importance next to one another.
- Coordinate design and source structure so screen readers follow the intended reading order.
- On the web, do not rely on CSS placement to establish screen reader order.

## Web landmarks and headings

Use landmarks to represent major content areas.

| Landmark | Use |
| --- | --- |
| navigation | Navigation links. Distinguish repeated instances with labels. |
| search | Search field |
| main | Main content. Use one. |
| banner | Repeated header content. Use one. |
| complementary | Supporting content that can stand alone |
| contentinfo | Site and content information, typically the footer. Use one. |
| region | Important content block. Give every region a clear label. |
| form | Content that takes and stores user information |

- Give repeated landmarks clear, specific labels. Do not repeat the landmark role in the label.
- Add a landmark label when it improves meaning.
- Assign headings from content hierarchy, rather than visual styling.
- Use H1–H6 in sequential levels. Do not skip a level.
- Prefer one H1 for the page title.
- Use meaningful heading titles. Change unclear titles or add an assistive-technology label.

## Interaction targets

- For most platforms, consider touch targets of at least 48 × 48dp.
- A 24 × 24dp icon can sit inside a 48 × 48dp target.
- The recommended physical touch size is 7–10mm. Larger targets may suit more users.
- The source notes an iOS recommendation of 44 × 44dp.
- Consider pointer targets of at least 44 × 44dp.
- In most cases, separate targets by at least 8dp.

## Verify structure

Check reading order, heading levels, landmark labels, and target bounds separately from visual styling.
