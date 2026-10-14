---
name: m3-styles-icons-application
description: Apply and verify Material Symbols styles, variable axes, text alignment, labels, targets, and localization.
---

# Icon application

Use only the directions from the supplied Material 3 sources. Do not invent missing values or behavior.

Read [source details](references/source-map.md) for section links, source tables, diagrams, and token modules.

Source: [Icons: Overview](https://m3.material.io/styles/icons).

Source: [Icons: Applying icons](https://m3.material.io/styles/icons/applying-icons).

## Select and style symbols

- Use Material Symbols as the default icon set.
- Choose outlined, rounded, or sharp styles consistently with product typography and shapes.
- Keep symbols filled when recognition requires it, such as full-body human or proprietary symbols.
- Use the variable font for adjustable weight, fill, grade, and optical size.
- Keep weights consistent. At 24dp, use at least weight 200.
- Use regular weight 400 as the baseline. Avoid excessive weight at 24dp.
- Use fill 0 for unfilled and fill 1 for filled states.
- Use fill changes to communicate state transitions when appropriate.
- Use grade for finer thickness adjustments with less effect on symbol size.
- Use grade 0 for dark icons on light backgrounds and -25 for light icons on dark backgrounds.
- Use positive grade when an active state needs heavier strokes.
- Set optical size within 20dp–48dp to preserve appearance during resizing.
- Use 20dp optical size for dense desktop layouts and 40dp–48dp for highlighted primary actions.

## Pair symbols with text

- Match the symbol and text size and optical weight.
- Where available, match compatible text and symbol grade values.
- Shift the symbol baseline downward by approximately 11.5% of the text size.

## Support comprehension and interaction

- Give abstract symbols short, meaningful labels.
- Provide labels for navigation items.
- Use unlabeled icons cautiously. Their meaning must remain unambiguous and accessible.
- Below 20dp, label complex icons and icons for key actions.
- Simple symbols may appear alone at smaller sizes only while identifiable.
- Give 24dp symbols a 48dp target by default.
- For primary mouse and keyboard input, a 20dp symbol may use a 40dp target.
- Keep sufficient surrounding space for recognition and interaction.

## Verify localization

Test icons across age groups, cultures, languages, and levels of technical familiarity.
Adapt symbols to local conventions, such as cart, bag, or basket.
Check local meanings of colors and symbols.
