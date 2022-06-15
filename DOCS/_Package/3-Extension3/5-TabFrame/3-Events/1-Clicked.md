---
layout: default

grand_parent: TabFrame Class
parent: Events
has_children: false
title: Clicked Event
nav_order: 1
permalink: /package/extension3/tabframe/events/clicked
---
# {{ page.title }}
<br>
Occurs when the left mouse button is clicked.

The following child objects are attached to the Event object.

| Type   | Name           | Description                                |
|--------|----------------|--------------------------------------------|
| Number | **_ShiftKey_** | 1 if the Shift key is pressed, 0 otherwise |
| Number | **_CtrlKey_**  | 1 if the Ctrl key is pressed, 0 otherwise  |
| Number | **_AltKey_**   | 1 if the Alt key is pressed, 0 otherwise   |
| Number | **_xPos_**     | X coordinate of mouse pointer              |
| Number | **_yPos_**     | Y coordinate of mouse pointer              |

Example
```
Function OnClicked(e) {
    MessageBox(strf("(%1,%2)でクリックされました", e.xPos, e.yPos));
}
```