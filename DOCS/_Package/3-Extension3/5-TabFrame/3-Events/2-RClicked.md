---
layout: default

grand_parent: TabFrame Class
parent: Events
has_children: false
title: RClicked Event
nav_order: 2
permalink: /package/extension3/tabframe/events/rclicked
---
# {{ page.title }}
<br>
Occurs when the right mouse button is clicked.

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
Function OnRClicked(e) {
    MessageBox(strf("(%1,%2)で右クリックされました", e.xPos, e.yPos));
}
```