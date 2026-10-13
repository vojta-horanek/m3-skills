---
name: m3-foundation-color-contrast
description: Apply and verify Material 3 contrast guidance for text, meaningful imagery, clustered controls, standalone controls, and disabled states.
---

# Color contrast

## Contrast requirements

Source: [Color contrast](https://m3.material.io/foundations/designing/color-contrast).

Use contrast to make content, controls, and actions distinguishable, including in bright or low light.

| Content | Minimum contrast against background |
| --- | --- |
| Small text | 4.5:1 |
| Large text, at least 14pt bold or 18pt regular | 3:1 |
| Graphics | 3:1 |

- Disabled states do not need to meet contrast requirements.
- Some non-text containers, such as buttons, should meet 3:1 against the surrounding background.
- In a cluster, each component container should reach at least 3:1 against the background.
- A prominent standalone component, such as a FAB, does not need that container-to-background minimum.
- Keep this standalone exception specific to container contrast. It does not waive text contrast guidance.

## Images containing information

Source: [Writing best practices](https://m3.material.io/foundations/writing/best-practices).

- Apply text contrast requirements to essential text in informative imagery.
- Distinguish essential information from decoration. Non-informative decorative elements do not need the same contrast requirements.

## Verify contrast

Check text and essential graphics against their backgrounds.
Check every clustered container separately.
Account for disabled states and the specific standalone-container exception.
