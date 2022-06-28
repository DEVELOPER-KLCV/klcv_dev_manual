---
layout: default

grand_parent: ListView Class
parent: Events
has_children: false
title: RClicked Event
nav_order: 4
permalink: /package/extension4/listview/events/rclicked
---
# {{ page.title }}

Occurs when the right mouse button is clicked.

The following child objects are attached to the Event object.

| Type   |     Name     | Description                                |
|--------|:------------:|--------------------------------------------|
| Number | **_ShiftKey_** | 1 if the Shift key is clicked, 0 otherwise |
| Number |  **_CtrlKey_** | 1 if the Ctrl key is clicked, 0 otherwise  |
| Number |  **_AltKey_**  | 1 if the Alt key is clicked, 0 otherwise   |
| Number |   **_xPos_**   | X coordinate of mouse pointer              |
| Number |   **_yPos_**   | Y coordinate of mouse pointer              |

Usage Example

```
Function OnRClicked(e) {
    MessageBox(strf("(%1,%2)で右クリックされました", e.xPos, e.yPos));
}
```