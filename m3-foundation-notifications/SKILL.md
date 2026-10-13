---
name: m3-foundation-notifications
description: Design, write, or verify Material 3 notifications and SMS for relevance, actionability, timing, character limits, and user controls.
---

# Notifications

Source: [Notifications](https://m3.material.io/foundations/content-design/notifications).

## Purpose and timing

- Focus on the user. Make notifications precise, timely, actionable, contextual, and relevant.
- Do not use notifications for unsolicited ads.
- Target users who benefit from the message. Consider segments, in-app behavior, and relevant personal information.
- Put the most important information first, including at the start of the title or sentence.
- Make next actions concise, specific, and clear. Include motivation when known.
- Do not repeat the app name or logo already supplied by the notification UI.
- Prefer useful, direct messages over jokes or excessive attempts at delight.
- Use weekdays instead of “today,” “tomorrow,” or “tonight.” Relative terms can suit notifications that auto-dismiss at a set timestamp.
- Do not trigger onboarding-related messages during onboarding.
- Provide contextual opt-out controls. Explain the benefit gained or lost through opt-in or opt-out.

## Dynamic text and limits

- Avoid dynamic text when possible, especially in titles. Translation can make it exceed the available space.
- Prefer dynamic text in the body.
- If a title needs dynamic text, pair it with no more than one additional word where possible.
- Provide a shorter backup when the primary version exceeds the character count.
- A truncated title does not expand even when the notification body expands.

| Part | Suggested limit |
| --- | --- |
| Title | Fewer than 29 characters |
| Collapsed body | Fewer than 40 characters |
| Expanded body | Fewer than 80 characters. Start with the collapsed body and add detail. |
| Actions | 1–2 buttons, with 1–2 words each |

## SMS and emoji

- Use SMS for important or urgent communication.
- Keep Latin-language SMS below 160 characters and non-Latin-language SMS below 134 characters, as specified by the source.
- Tell translators about the limits in the message description.
- Avoid unnecessary full email addresses and website links that consume space.
- Use emoji sparingly to enhance words, rather than replace them.
- Account for cultural differences in emoji meanings.
- Do not use negative emoji to accentuate bad news.

## Verify messages

Check relevance, front-loaded meaning, next actions, timing, opt-out access, and character counts with dynamic text and translations.
