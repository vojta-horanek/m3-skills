---
name: m3-foundation-inputs
description: Design, implement, or verify Material 3 mouse, trackpad, stylus, physical keyboard, touch, and mixed-input behavior.
---

# Inputs

Source: [Inputs](https://m3.material.io/foundations/interaction/inputs).

## Multiple input methods

- Support touch, keyboard, and mouse across device types and screen sizes.
- Account for external inputs on phones, tablets, foldables, TVs, laptops, and desktops.
- Support familiar input behavior when external devices connect.
- Show a mouse cursor when a mouse is used, including on touch devices.
- A mouse click or stylus tap should give feedback equivalent to touch, such as a pressed ripple.
- Use secondary click to open a context menu with options for the clicked object.
- Show hover changes on interactive objects and tooltips where applicable.

## Cursors and text selection

| Context | Cursor or interaction |
| --- | --- |
| Default external input | Pointer |
| Link or linked image | Hand |
| Resizable boundary | Resize arrows |
| Selectable or editable text | I-beam |
| Stylus tool properties | Cursor only when useful, such as brush size or shape |

- In editable text, a single click positions the cursor. A double click selects a word. A triple click selects a paragraph.
- A single click can deselect text and reposition the cursor.
- Highlight mouse, trackpad, or stylus selections with one color. Do not add touch controls beside those selections.
- For touch selection, show touch controls even when external inputs are connected.
- For mouse, trackpad, or stylus selection, use the I-beam and context menu even on a touch device.
- Touch dragging scrolls a text area. Mouse dragging selects its text.

## Scrolling and keyboards

- Let the wheel and two-finger trackpad gestures scroll the list under the cursor.
- Support horizontal fields with mouse-wheel scrolling and horizontal two-finger trackpad gestures.
- Support trackpad pinch for zooming.
- Let a physical keyboard perform the virtual keyboard's actions and additional keyboard actions.
- Hide the virtual keyboard when a physical keyboard is attached. Show it when that keyboard is removed.
- Use Enter for expected actions such as sending a message.
- Use Space or available media keys for expected play and pause actions.
- Make Tab order logical, generally left to right and top to bottom.
- Show a ring-like keyboard focus indicator on keyboard-focused interactive elements.
- Let Escape dismiss visible modal elements, remove focus, or clear selections as appropriate.
- When Escape removes a text cursor, preserve the text already entered.

## Verify inputs

Check pointer feedback, context menus, text selection, scrolling, keyboard attachment, focus visibility, and expected keyboard actions.
Check mixed-input behavior against the active input, rather than the device category alone.
