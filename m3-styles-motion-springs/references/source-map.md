# Spring motion: source details

Publisher: Google Material Design. Extraction date: October 14, 2026.
Content version: `2026-09-23_06-10-05`.

The public site loads its page sections from the linked content files.

## Motion physics system

Page update: `2026-07-17T05:25:55.367Z`.
[Public content file](https://m3.material.io/_dsm/content/m3/2026-09-23_06-10-05/ccf2c3e9-82b5-4c4a-9570-b0d08d95c0c1.json).

### How it works

[Supplied resource](https://m3.material.io/styles/motion/overview).

#### Source tables

These tables preserve the values and platform distinctions supplied in the page text.

| Type | Link | Status |
| --- | --- | --- |
| Implementation | Android Views (MDC-Android) | Available. Not added to components. See specs |
| Implementation | Flutter | Unavailable |
| Implementation | Jetpack Compose | Available |
| Implementation | Web | Compatible with Compose springs. See specs |

| Speed | Spatial example | Effects example |
| --- | --- | --- |
| Default | Animations that partially cover the screen, such as bottom sheet and expanded navigation rail | Opacity of the content within a navigation rail |
| Fast | Small components, such as switches and buttons | Color change of the switch handle |
| Slow | Full-screen animations | Full-screen content refresh |

#### Links published on the source page

These links identify source resources. Their destination content adds no requirements to this skill.

- [More on M3 Expressive](https://m3.material.io/blog/building-with-m3-expressive)
- [Android Views (MDC-Android)](https://github.com/material-components/material-components-android/blob/master/docs/theming/Motion.md)
- [See specs](https://m3.material.io/styles/motion/overview/specs)
- [Jetpack Compose](https://developer.android.com/reference/kotlin/androidx/compose/material3/MotionScheme)

#### Source diagrams and demonstrations

Read relevant diagrams for image-only specifications. Keep examples and incorrect examples distinct.

- [1. Showcase of expressive components and motion curves.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm9d3dbjl-00_Hero%20Expressive%20New_Export.mp4?alt=media&token=8e65768c-f1ca-4bc8-8738-36ca6ca76a2e)
- [2. The expressive motion scheme overshoots the final values to add bounce](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g74buu-00_Scheme_Spring%20Expressive%20Export.mp4?alt=media&token=36db86e1-4e85-4905-89fb-f82c1fa64091)
- [3. The standard motion scheme eases into the final values](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g75t7b-00_Scheme_Spring%20Standard%20Export.mp4?alt=media&token=37eb508f-ab3e-42e7-8491-1eac28f85f3a)
- [4. All component motion is driven by two tokens: expressive fast spatial and expressive fast effects](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g79o8z-00_Versatile%20Export.mp4?alt=media&token=5fa65ca6-0cb0-470a-8856-841efe260166)
- [5. Each scheme (expressive, standard) has three speeds (fast, default, slow) for two types of movement (spatial, effects)](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm8or28vc-5.png?alt=media&token=12806c6a-d624-4706-87bf-91cc61506aa1)
- [6. Spatial springs apply to movement](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g7et1l-00_Tokens%20Spatial%20Pos%20Export.mp4?alt=media&token=589eb77a-314a-4fb3-917f-5ca18dcc1fd5)
- [7. Spatial springs apply to rotation](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g8hvpt-00_Tokens%20Spatial%20Rotation%20Export.mp4?alt=media&token=8515f662-83e8-4a7c-92b1-b796942741e4)
- [8. Effects springs applied to opacity](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g8j35o-00_Tokens%20Effects%20Opacity%20Export.mp4?alt=media&token=b6ff1430-d858-4053-bbbb-bac2d4dc9ca8)
- [9. Effects springs applied to color](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g8k2bk-00_Tokens%20Effects%20Color%20Export.mp4?alt=media&token=eb6350cb-81b8-410c-b991-1ccbad5c7079)
- [10. Spatial motion in fast, default, and slow speeds](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g8v98f-00_AllSpeeds_Expressive%20Export.mp4?alt=media&token=e2706336-378f-4bd8-a5bb-5e0708fd9338)
- [11. Effects motion in fast, default, and slow speeds](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g8u69a-00_AllSpeeds_Standard%20Export.mp4?alt=media&token=875faef0-4f97-4143-9839-cc66fc6d51ac)
- [12. Material components use the physics motion system to feel more expressive](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g8ypfu-00_Components%20Export.mp4?alt=media&token=7a1812c2-c6a8-458b-bec1-840659b329f0)
- [13. Switch using the expressive motion scheme](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g90urt-00_Customization%20Switch%20Expressive%20Export.mp4?alt=media&token=431a79da-59d7-445e-96cc-23be15820673)
- [14. Switch using the standard motion scheme](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0qp1jmp-00_Customization%20Switch%20Standard%20Export.mp4?alt=media&token=d914f315-63fd-4f3a-991a-c279d6e97e6b)
- [15. FAB menu with an extra stiff custom scheme](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g93afq-00_Customization%20Fab%20Instant%20Export.mp4?alt=media&token=929f4440-1e93-4437-8234-a587c30a6542)
- [16. FAB menu with very low stiffness custom scheme](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fm0g946r2-00_Customization%20Fab%20Soft%20Export.mp4?alt=media&token=37c06170-cc10-4273-94db-5e7ab434c3a6)

### Specs

[Supplied resource](https://m3.material.io/styles/motion/overview/specs).

#### Source tables

These tables preserve the values and platform distinctions supplied in the page text.

| Platform | Status | How to apply |
| --- | --- | --- |
| Jetpack Compose | Available | Use built-in components and spring tokens. |
| Android Views (MDC-Android) | Available. Not added to components. | Use built-in spring tokens. |
| Web | Compatible | Use springs when possible, otherwise use curves that mimic the springs for animations without interruptions or gestures. View web conversion table |

| Spring | Curve |
| --- | --- |
| Expressive fast spatial | 0.42, 1.67, 0.21, 0.90. Duration = 350ms |
| Expressive default spatial | 0.38, 1.21, 0.22, 1.00. Duration = 500ms |
| Expressive slow spatial | 0.39, 1.29, 0.35, 0.98. Duration = 650ms |
| Expressive fast effects | 0.31, 0.94, 0.34, 1.00. Duration = 150ms |
| Expressive default effects | 0.34, 0.80, 0.34, 1.00. Duration = 200ms |
| Expressive slow effects | 0.34, 0.88, 0.34, 1.00. Duration = 300ms |
| Standard fast spatial | 0.27, 1.06, 0.18, 1.00. Duration = 350ms |
| Standard default spatial | 0.27, 1.06, 0.18, 1.00. Duration = 500ms |
| Standard slow spatial | 0.27, 1.06, 0.18, 1.00. Duration = 750ms |
| Standard fast effects | 0.31, 0.94, 0.34, 1.00. Duration = 150ms |
| Standard default effects | 0.34, 0.80, 0.34, 1.00. Duration = 200ms |
| Standard slow effects | 0.34, 0.88, 0.34, 1.00. Duration = 300ms |

#### Token modules

Open the supplied page to select the applicable token set and platform context.
The content file identifies these modules but does not include their dynamically loaded values.
Do not replace unavailable values with estimates.

- Resource: `designSystems/20543ce18892f7d9`.
  Type: `TOKEN_TYPE_UNSPECIFIED`.
  Configuration: `{"tokenSets": ["Motion"], "contextTags": ["Standard", "Expressive", "Compose", "Web", "Android"]}`.
