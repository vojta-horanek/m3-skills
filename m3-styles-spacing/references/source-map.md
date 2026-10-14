# Spacing: source details

Publisher: Google Material Design. Extraction date: October 14, 2026.
Content version: `2026-09-23_06-10-05`.

The public site loads its page sections from the linked content files.

## Spacing

Page update: `2026-07-17T05:30:24.800Z`.
[Public content file](https://m3.material.io/_dsm/content/m3/2026-09-23_06-10-05/36e81931-9b87-406f-9ec5-c0cc049564d8.json).

### Overview

[Supplied resource](https://m3.material.io/styles/spacing).

#### Source tables

These tables preserve the values and platform distinctions supplied in the page text.

| Type | Resource | Status |
| --- | --- | --- |
| Implementation | Android Views (MDC-Android) | Unavailable |
| Implementation | Jetpack Compose | Available |
| Implementation | Web | Unavailable |

#### Source diagrams and demonstrations

Read relevant diagrams for image-only specifications. Keep examples and incorrect examples distinct.

- [1. Spacing should adapt to component size, layout, form factor, and other contexts](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp45pjnu-01.png?alt=media&token=4bc20db7-589b-4e9f-8a41-6ef0912181bf)
- [2. Spacing units are are created as a multiplier from the baseline unit of 8dp, which is space100](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp46hu30-02.png?alt=media&token=8c945825-e613-4d44-8b78-754d4f368664)
- [3. Spacing concepts for components: Vertical padding (top & bottom) Vertical gap Horizontal padding (leading & trailing) Horizontal gap](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp46iygv-03.png?alt=media&token=1ffbf4cf-d3d8-492a-bf87-543363d09c2a)
- [4. Spacing concepts for layouts: Margin Top padding Horizontal padding (leading & trailing) Spacer (gap) Vertical gap](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp46qg1t-04.png?alt=media&token=de6ad9a3-9fd4-419c-afb9-845b48380977)
- [5. Search horizontal margins are 24dp by default to ensure accurate placement from the screen edge](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp46u5o7-05.png?alt=media&token=ec9f8771-d0f9-40dc-bda9-5de5123f3961)
- [6. Search margins change to 12dp when focused, while the container padding and horizontal gaps remain the same](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp46ujx2-06.png?alt=media&token=117fe589-68f0-4c73-b242-a6f6e0970b13)
- [7. Padding can be horizontal or vertical, or on a specific edge: leading, trailing, top, or bottom](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmpcmizsr-07.png?alt=media&token=64b66712-c4a1-49fc-96a2-462fbe2cb910)
- [8. Gaps can be horizontal, vertical, or defined by the elements around it](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp46wxwi-08.png?alt=media&token=2aa763aa-37db-4c60-8ebe-ed2c068891ac)
- [9. Margins can be horizontal or vertical, or on a specific edge: leading, trailing, top, or bottom](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp46ywq1-09.png?alt=media&token=c7d6c7ca-77f2-4f73-b0bb-1f47c60f09c1)
- [10. Define padding and gaps on the parent container to organize all elements inside](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp46yjrr-10.png?alt=media&token=7a66f957-b8d4-491d-939a-1bac71e540c7) — Source marker: DO.
- [11. Avoid defining margins on child elements as they usually aren’t uniform, and require more tokens](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp46z9b3-11.png?alt=media&token=16464639-7f1c-4c21-a46b-7126cd037463) — Source marker: DON'T.

### Applying spacing

[Supplied resource](https://m3.material.io/styles/spacing/applying-spacing).

#### Source diagrams and demonstrations

Read relevant diagrams for image-only specifications. Keep examples and incorrect examples distinct.

- [1. Components have padding tokens that map to system tokens, which resolve to final values](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp472g1b-01.png?alt=media&token=faa1b24c-a165-4354-b169-fc162674a082)
- [2. Many Material components map to spacing system tokens](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp475gv4-02.png?alt=media&token=d9282ad6-6edc-49c7-898d-1ee6447ccdb3)
- [3. System tokens define all spacing values recommended by Material](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp475tmf-03.png?alt=media&token=267b98d3-faa5-422e-82b5-611308686964)
- [4. Keep the same spacing when text scales](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp4783qn-04.png?alt=media&token=430e5fcc-38c8-4834-ad99-b2f9cd77b880)
- [5. Customize component spacing to change it across the entire product](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp47e5lm-08.png?alt=media&token=4125df00-d67d-414f-8c2e-1bf678da66d3)
- [6. For products that adapt spacing the exact same way, consider creating a token for that pattern](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp47j8c0-09.png?alt=media&token=6645788e-b661-4525-a3e8-ceeb553432a6)
- [7. Components can be customized to adapt spacing to each form factor](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp47k75s-GM3%20-%20Spacing%20-%20Applying%2001%20-%20%20IA%20-%20v01.mp4?alt=media&token=dd6dc0fc-646f-4a8c-8afe-86bb6f067126)
- [8. Components can be customized to adapt spacing to density settings](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp47kp67-GM3%20-%20Spacing%20-%20Applying%2002%20-%20%20IA%20-%20v01.mp4?alt=media&token=59436e7e-acc6-412f-a59d-d6ca2aba340d)

### Tokens

[Supplied resource](https://m3.material.io/styles/spacing/tokens).

#### Token modules

Open the supplied page to select the applicable token set and platform context.
The content file identifies these modules but does not include their dynamically loaded values.
Do not replace unavailable values with estimates.

- Resource: `designSystems/20543ce18892f7d9`.
  Type: `MEASUREMENT`.
  Configuration: `{"tokenSets": ["Spacing"], "tokenSetOrder": ["Spacing", "State - focus indicator"]}`.

#### Source diagrams and demonstrations

Read relevant diagrams for image-only specifications. Keep examples and incorrect examples distinct.

- [1. The main spacing units are multiples of 8dp](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp47oayx-01.png?alt=media&token=6b2b9e59-81db-4010-9252-c23b0029f8d1)
- [2. Material only defines nested units that are actively used in common layouts or Material components](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmp47p71x-01.png?alt=media&token=f8dfa98b-3b66-41ad-a923-ca87b3686549)
