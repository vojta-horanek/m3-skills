# Elevation: source details

Publisher: Google Material Design. Extraction date: October 14, 2026.
Content version: `2026-09-23_06-10-05`.

The public site loads its page sections from the linked content files.

## Elevation

Page update: `2026-07-17T05:03:59.318Z`.
[Public content file](https://m3.material.io/_dsm/content/m3/2026-09-23_06-10-05/38354be9-206b-4988-96a8-0f2a88074511.json).

### Overview

[Supplied resource](https://m3.material.io/styles/elevation).

#### Source tables

These tables preserve the values and platform distinctions supplied in the page text.

|  | Resource | Status |
| --- | --- | --- |
| Design | Design Kit (Figma) | Available |
| Implementation | Flutter | Available |
|  | Jetpack Compose | Available |
|  | MDC - Android | Available |
|  | MWC - Web | Available |

#### Links published on the source page

These links identify source resources. Their destination content adds no requirements to this skill.

- [Design Kit (Figma)](https://www.figma.com/community/file/1035203688168086460)
- [Flutter](https://api.flutter.dev/flutter/material/ElevationOverlay-class.html)
- [Jetpack Compose](https://developer.android.com/develop/ui/compose/designsystems/material3?_gl=1*zh4ff1*_up*MQ..*_ga*MTQ4NTEwOTIzLjE3NDA0MDY2Njk.*_ga_6HH9YJMN9M*MTc0MDQwNjY2OC4xLjAuMTc0MDQwNjY2OC4wLjAuNjU3NTAyNDY.#elevation)
- [MDC - Android](https://github.com/material-components/material-components-android/blob/d56070586102b66486f7f8697de077c3d7689922/docs/theming/Color.md#using-surface-colors)
- [MWC - Web](https://github.com/material-components/material-web/blob/919fe12badcfee4dcd72c390c0869dd8f996b51c/docs/components/elevation.md)

#### Source diagrams and demonstrations

Read relevant diagrams for image-only specifications. Keep examples and incorrect examples distinct.

- [1. Elevation represents the distance between elements. The product applies color to represent elevation. One surface at 1dp elevation and another surface at 8dp elevation, as viewed from the front The difference in elevation between the two surfaces is 7dp, as viewed from the side](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwykafum-1.png?alt=media&token=686eda7a-aed0-4d34-a749-0b01f2a50a86)
- [2. M2: Shadows applied at all levels](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwykc8yv-2.png?alt=media&token=7c4a4e4e-ff37-47d2-a375-579c3f945893)
- [3. M3: Using color instead of shadows to communicate elevation](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwykckey-3.png?alt=media&token=fd1c5548-7048-4d2c-9123-17308e339731)
- [4. Elevation can be depicted using shadows or other visual cues, such as surface fills with a tone difference](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwykjf69-GM3-Styles-Elevation-Overview-1-v01.mp4?alt=media&token=6a6f026f-2264-474b-9b2d-cab3cd08393e)
- [5. All components have a default elevation which should be used](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwykcxkh-5.png?alt=media&token=d0b226cf-0e17-4719-9f5c-8a186936d003)
- [6. Hovering over a button increases its elevation to show user interaction](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwykkk4p-GM3-Styles-Elevation-Overview-2-v01.mp4?alt=media&token=8ca50f54-913b-4e5a-9e22-22c99a867fd2)

### Applying elevation

[Supplied resource](https://m3.material.io/styles/elevation/applying-elevation).

#### Source diagrams and demonstrations

Read relevant diagrams for image-only specifications. Keep examples and incorrect examples distinct.

- [1. Material uses six levels of elevation, each with a corresponding dp value. These values are named for their relative distance above the UI’s surface: 0, +1, +2, +3, +4, and +5. An element’s resting state can be on levels 0 to +3, while levels +4 and +5 are reserved for user-interacted states such as hover and dragged.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwyl8vgl-1.png?alt=media&token=d090e3a9-52f9-46c7-b341-3bd6ea781fdd)
- [2. Two overlapping surfaces with distinct tonal values Two overlapping surfaces with the same tonal values separated via shadow Two overlapping surfaces with the same tonal values separated via scrim](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwyl9cz5-2.png?alt=media&token=731fe08f-ab2d-4a21-9ee1-2e963425c39a)
- [3. A FAB's elevation helps separate it from body content A scrim appears below a modal to communicate importance Tonal differences between a navigation bar and body content indicate separate surfaces](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwynetr7-3.png?alt=media&token=d733e384-21d7-432c-a68d-917f362b91a2)
- [4. Ensure floating elements have sufficient contrast with surfaces beneath](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwynhr1z-5_do.png?alt=media&token=a4718cb7-4b12-442d-a48a-1baab845cc2f) — Source marker: DO.
- [5. Don't use colors with insufficient contrast. The relationship between surfaces must be clear.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwyni1qa-4_dont.png?alt=media&token=82bf3fa0-c8a8-48df-b10c-1b5c265cdc20) — Source marker: DON'T.
- [6. Surface Surface container](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwynjnhh-6.png?alt=media&token=9e184a9c-6448-4ef4-9bea-c512f807b8d9)
- [7. Smaller, sharper shadows indicate a surface’s close proximity to the surface behind it](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwynkcgy-7.png?alt=media&token=faa5a587-cb71-4402-b4e3-5c7c598fc84f)
- [8. Larger, softer shadows express more distance between a surface and the one behind it](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwynkpp5-8.png?alt=media&token=97f08517-0310-4ac0-bfdd-e76abf2a451b)
- [9. Interactive elements are emphasized with elevation](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwynle77-9.png?alt=media&token=da60b0e7-2216-4d40-bbab-d5359875d09c)
- [10. Elevation encourages interaction](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwynmywr-GM3-Styles-Elevation-Applying_Elevation-1-v01.mp4?alt=media&token=d25ea774-8c2d-4a56-ae20-59c0691d4cb8)
- [11. Scrims help bring focus to important elements like the navigation rail](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flwynlv1e-11.png?alt=media&token=a29315d8-497f-4376-8018-f661ea795b3a)

### Tokens

[Supplied resource](https://m3.material.io/styles/elevation/tokens).

#### Source tables

These tables preserve the values and platform distinctions supplied in the page text.

| Resting level | Component | DP Height |
| --- | --- | --- |
| 5 | (not assigned as resting level) | 12dp |
| 4 | (not assigned as resting level) | 8dp |
| 3 | Date pickers / Dialogs (modal) / Extended FAB / FAB / FAB menu (close button) / Search / Time pickers | 6dp |
| 2 | App bar (scrolled) / Menu / Navigation bar / Rich tooltip / Toolbar | 3dp |
| 1 | Banner / Bottom sheet (modal) / Button (elevated) / Card (elevated) / Chips (elevated) / Navigation drawer (modal) / Side sheet (modal) | 1dp |
| 0 | App bar (not scrolled) / Buttons (filled, tonal, outlined) / Button groups / Cards (filled, outlined) / Carousel / Chips / Dialog (full-screen) / Extended FAB (in navigation rail) / FAB (in navigation rail) / FAB menu (list items) / Icon buttons / List / Navigation rail / Segmented button / Side sheet (docked) / Slider / Split button / Tabs | 0dp |

#### Token modules

Open the supplied page to select the applicable token set and platform context.
The content file identifies these modules but does not include their dynamically loaded values.
Do not replace unavailable values with estimates.

- Resource: `designSystems/20543ce18892f7d9`.
  Type: `ELEVATION`.
  Configuration: `{"contextTags": ["None", "Medium contrast", "Default", "High contrast", "3P", "Android", "Dark", "Light"]}`.
