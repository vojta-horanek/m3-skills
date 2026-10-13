---
name: m3-foundation-rtl
description: Design, implement, or verify Material 3 right-to-left layouts, text direction, mirrored controls, gestures, and locale-specific exceptions.
---

# Bidirectionality and RTL

Source: [Bidirectionality and RTL](https://m3.material.io/foundations/layout/bidirectionality-rtl).

## Layout and text

- Support LTR and RTL through mirroring and correct text rendering.
- Use leading and trailing relationships instead of assuming fixed left and right positions.
- In RTL layouts, reading starts at the upper right, and mirrored elements change alignment and order.
- Handle text alignment and text directionality separately. RTL content generally needs right alignment and RTL flow.
- Check text entry, cursor placement, punctuation, phone numbers, URLs, and mixed-direction content.
- Keep an email domain to the right of its username. The username can still use RTL text and cursor movement.
- Mirror feed, list-detail, and supporting-pane arrangements.
- Mirror app bar arrangements and toolbar tool order.
- Put navigation rails on the leading edge, which is the right for RTL.
- Move badges to the mirrored position, such as the upper left of an icon.
- Keep chip trailing icons at the end of their container, which is the left for RTL.

## Icons, time, and exceptions

- Mirror directional icons such as back, forward, and send.
- Help icons mirror in some languages, including Urdu and Persian. Icon meaning can depend on culture.
- Do not mirror every graphic automatically. Graphs and charts retain LTR direction in Persian and Urdu.
- Linear progress generally moves right to left in RTL, except Hebrew, where it remains LTR.
- Hebrew timelines retain LTR direction.
- Media player controls for video and audio always remain LTR.
- Circular time representations and progress remain unchanged.
- Clocks remain clockwise and time direction stays LTR.
- In 12-hour RTL clocks, put AM/PM symbols on the left.
- Do not mirror clock icons, clockwise refresh icons, or clockwise-arrow progress indicators.

## Gestures

- Mirror swipe gestures and the actions they reveal.
- On Android, mirror predictive-back presentation for RTL.

## Verify RTL

Check mirrored structure and gestures alongside text alignment and directionality.
Check mixed-direction strings and the specific chart, Hebrew, media, and clock exceptions.
