---
name: m3-styles-typography-application
description: Apply and verify Material 3 type roles, platform typesetting, readability, number alignment, contrast, and links.
---

# Apply type

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read [source details](references/source-map.md) for section links, source tables, diagrams, and token modules.

Source: [Typography: Applying type](https://m3.material.io/styles/typography/applying-type).

## Assign roles

- Use display for short, important text or numerals, especially on large screens.
- Use headline for short, high-emphasis text on smaller screens and primary content regions.
- Use title for short, medium-emphasis text and secondary regions.
- Use body for longer passages with fonts readable at small sizes.
- Avoid decorative or expressive fonts in body text.
- Use label for small functional text, component labels, and captions.
- Use label large for buttons.
- Use expressive title fonts cautiously and maintain readable spacing in expressive headlines.
- Set optical size to the intended text usage when available.

## Typeset for the platform

- On Web and applicable iOS layouts, use bounding boxes, line height, padding, and container measurements.
- Center text within its line-height box using equal half-leading above and below.
- Specify distances from fixed references such as container edges.
- On Android or platform-neutral specifications, use baseline-relative measurements.
- Measure multiline line height between consecutive baselines.
- For centering, specify center alignment instead of a baseline distance.
- Reconcile design-tool font metrics with the implementation.

## Preserve readability

- Use Material's type tokens for their intended sizes and roles.
- For larger title, headline, and display text, use the source's recommended line-height ratio of 1.2.
- For body and label text, use the source's recommended ratio around 1.5.
- Use tabular numbers in tables and frequently changing values such as clocks.
- Use on surface as the default text color or on surface variant as an alternative.
- Provide 3:1 contrast for large text and 4.5:1 for small text.
- Underline hyperlinks on surfaces.
- Use primary for hyperlinks or tertiary when links need less emphasis.

## Verify

Check role hierarchy, platform measurements, long passages, changing numbers, contrast, and link underlines.
