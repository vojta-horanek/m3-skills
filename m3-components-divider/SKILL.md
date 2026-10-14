---
name: m3-components-divider
description: Design, implement, test, or verify Material 3 content grouping, full-width and inset lines, vertical dividers, and decorative semantics.
---

# Dividers

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/divider/overview).

Use subtle dividers to group content only when open space cannot provide sufficient hierarchy.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/divider/guidelines).

- Use full-width dividers for larger unrelated sections or interactive versus non-interactive regions.
- Use full-width lines sparingly.
- Use inset dividers for related or nested content.
- Align inset lines with anchoring icons, avatars, or the leading content edge.
- When combining full-width and inset lines, keep their hierarchy consistent.
- Repetitive list formats may need only margins, without divider lines.
- Use vertical dividers to organize content on larger screens.

## Implement the specs

Source: [Specs](https://m3.material.io/components/divider/specs).

- Use the outline variant color role.
- Full-width dividers span 100%.
- Leading-inset dividers use 16dp leading margin and 0dp trailing margin.
- Middle-inset dividers use 16dp on both sides.
- The measurement table gives 4dp between divider and supporting text.
- Use the source diagram for its context-specific 8dp right and bottom margins.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/divider/accessibility).

Dividers are decorative elements. The source assigns them no minimum contrast requirement.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
