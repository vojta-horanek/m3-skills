---
name: m3-styles-typography-scale
description: Implement and verify Material 3 baseline and emphasized type tokens, custom scales, units, and language height support.
---

# Type scale and tokens

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read [source details](references/source-map.md) for section links, source tables, diagrams, and token modules.

Source: [Typography: Overview](https://m3.material.io/styles/typography).

Source: [Typography: Type scale & tokens](https://m3.material.io/styles/typography/type-scale-tokens).

## Select styles and tokens

- Use one scale with 15 baseline and 15 emphasized styles.
- Use display, headline, title, body, and label roles in large, medium, and small sizes.
- Select only the styles the product needs.
- Use composite style tokens for defaults and individual property tokens for targeted customization.
- Use baseline and emphasized styles together.
- Use emphasized styles for selection, primary actions, unread messages, headlines, or editorial emphasis.
- Do not assume components use emphasized styles by default.
- Swap a baseline token for the same emphasized role, such as md.sys.typescale.emphasized.display-large.

## Customize carefully

- Set brand typefaces for larger expressive styles and plain typefaces for smaller readable styles.
- Change brand and plain font tokens before refining line height and letter spacing.
- Avoid size changes during individual style refinement because they affect component rendering and reflow.
- Adjust both baseline and emphasized sets while keeping emphasized treatments visually consistent.
- Account for weight, ascenders, and descenders when adjusting spacing and line height.
- When a different scale is necessary, add, remove, or resize styles deliberately.
- Use clear size differences. The source uses a Major Second ratio of 1.125 with base size 14.
- Account for the possibility that custom tokens no longer receive Material typography updates.

## Support language height

- Default to medium language height and switch based on detected language.
- Use small for Cyrillic, Greek, Hebrew, and Latin-based scripts except Vietnamese.
- Use medium for the source's listed scripts and most other languages.
- Use large for Burmese and Telugu.
- Use extra large for Nastaliq.
- Let vertically padded components adapt to language height.
- Check fixed-height components explicitly. They may not adapt by default.
- Open the line-height folder and select the language-height context in the token module.

## Apply units and verify

Use sp on Android and rem on Web.
At a 16px root size, convert a font size with SP_SIZE / 16 = rem.
Read the source tables for letter-spacing units and examples before conversion.
Check both style sets, language categories, clipping, overlap, and component reflow.
