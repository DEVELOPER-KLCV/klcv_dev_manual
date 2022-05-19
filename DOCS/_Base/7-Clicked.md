---
layout: default
has_children: true

title: Clicked Event
nav_order: 7
permalink: /base/clicked
has_toc: false
---

# {{ page.title }}

Occurs when the left mouse button is pressed.

The following child objects are attached to the Event object.

| Type   | Name       | Description                                |
|--------|------------|--------------------------------------------|
| Number | ShiftKey   | 1 if the Shift key is pressed, 0 otherwise |
| Number | CtrlKeyKey | 1 if the Ctrl key is pressed, 0 otherwise  |
| Number | AltKey     | 1 if the Alt key is pressed, 0 otherwise   |
| Number | xPos       | X coordinate of mouse pointer              |
| Number | yPos       | Y coordinate of mouse pointer              |

Example of use
```
Function OnClicked (e) {
    MessageBox (strf (" clicked on (% 1,% 2) ", e.xPos, e.yPos));
}
```