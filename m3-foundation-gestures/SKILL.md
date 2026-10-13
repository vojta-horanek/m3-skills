---
name: m3-foundation-gestures
description: Design, implement, or verify Material 3 touch gestures, real-time responses, compound gestures, and Android predictive back.
---

# Gestures

Source: [Gestures](https://m3.material.io/foundations/interaction/gestures).

Make UI elements respond to gestures in real time.
Use gestures to navigate, take action, or transform content.

| Gesture | Use described by Material |
| --- | --- |
| Tap | Navigate to a destination or interact with an element |
| Double tap | Zoom content in or out |
| Long press | Access additional functionality, such as selecting an item |
| Scroll or pan | Move through surfaces vertically, horizontally, or in another direction |
| Swipe | Move between peer views or complete actions |
| Drag | Move elements or slide surfaces into and out of view |
| Long press and drag | Pick up and move content, including reordering |
| Pinch | Scale a surface, including transitions between views |
| Compound gesture | Transition between gestures, such as pan and pinch on a map |

## Predictive back

On Android, predictive back lets users preview navigation to the previous destination during a swipe.
Users can continue the gesture or stay in the current view before completing it.
The source lists bottom sheets, navigation bars, navigation rails, search bars, and side sheets as compatible components.

## Verify gestures

Check real-time response and the intended navigation, action, or content transformation.
Check that compound gestures transition fluidly.
For predictive back, check both continuation and cancellation before gesture completion.
