---
name: m3-components-badges
description: Design, implement, test, or verify Material 3 notification badges, item counts, anchoring, labels, and announcements.
---

# Badges

Use only the directions supported by the linked Material 3 sources. Do not infer missing measurements or behavior.

Read [source details](references/source-map.md) for source coverage, measurement diagrams, and token-table locations.

## Choose the component

Source: [Overview](https://m3.material.io/components/badges/overview).

Use small badges for unread notifications and large badges for counts or status.
Keep labels within four characters, including a plus sign.

## Design and behavior

Source: [Guidelines](https://m3.material.io/components/badges/guidelines).

- Use badges with navigation bars, rails, app bars, or tabs.
- Anchor badges inside the icon bounds at the upper trailing edge.
- Mirror badge placement for RTL languages.
- Let count badges expand without changing their anchor.
- Use the default badge colors.
- Use a small badge when space is tight or a large badge would collide with another element.
- Place large badges at the trailing edge when another element follows the icon.
- Do not let badges cover icons, collide with elements, or get clipped.
- Truncate labels when necessary to keep the four-character limit.
- In navigation bars, hide unread badges once the destination is selected.

## Implement the specs

Source: [Specs](https://m3.material.io/components/badges/specs).

- Use error for the badge container and on error for its label.
- Small badges measure 6dp with 3dp corner radii.
- One-digit large badges measure 16dp with 8dp corner radii.
- Maximum-character large badges measure 16×34dp.
- Small anchor offsets measure 6×6dp from the icon's top trailing corner to the badge's bottom leading corner.
- Large anchor offsets measure 14×12dp.
- Use 4dp between badge and text containers.

## Accessibility and verification

Source: [Accessibility](https://m3.material.io/components/badges/accessibility).

- Provide at least 3:1 contrast. Prefer the default mappings.
- Include badge information after the destination in screen reader announcements.
- Read the count for numeric badges.
- Announce New notification for non-counting badges.
- Let people address the notification by selecting its navigation destination.

## Verify

Check the applicable directions above against the application. Check each supported state, input method, and layout described here.
