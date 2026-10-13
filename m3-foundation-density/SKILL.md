---
name: m3-foundation-density
description: Design, implement, or audit Material 3 information density, component scaling, accessible density controls, and density-independent units.
---

# Density

Source: [Density](https://m3.material.io/foundations/layout/grids-spacing/density).

## Information and component density

- Distinguish information density from component scaling and screen pixel density.
- Use higher information density when people need to scan, view, or compare many items, such as tables, lists, or long forms.
- Change margins, spacers, and padding to adjust information density without necessarily scaling components.
- Consider whether higher density benefits the user and device context. Not every layout needs it.
- Do not automatically change a person's density setting across breakpoints or orientation changes.
- Component density starts at 0. Negative levels increase density.
- Higher component density typically reduces vertical padding or overall height in 4dp increments.
- Center grouped content within the component. Do not change text size when scaling its container.
- Do not increase density for focused selection tasks, such as menus, where smaller selectable areas reduce usability.
- Do not increase density in components that alert users to changes, such as snackbars or dialogs.

## Targets and controls

- Default interaction targets should be at least 48 × 48 CSS pixels.
- The source also states a 48 × 48dp minimum for accessible targets. Preserve the source's platform units.
- Do not apply component scaling by default when it produces targets below the default minimum.
- Let users opt into denser layouts and components.
- Keep density settings controls at default target size so users can revert the setting easily.
- Smaller visible icons or containers can retain larger interactive targets.
- Use caution with increased density that reduces selectable space.

## Screen units

- Pixel density is the number of pixels per inch.
- Calculate density as screen width or height in pixels divided by the same dimension in inches.
- Use density-independent pixels to keep physical dimensions consistent across screen densities.
- At a screen density of 160, one dp equals one physical pixel.
- Calculate dp as `(pixels × 160) / screen density`.

## Verify density

Check text size, interactive target bounds, accessible settings controls, and preservation of the user's chosen density.
Check whether denser content improves comparison without reducing focused-task usability.
