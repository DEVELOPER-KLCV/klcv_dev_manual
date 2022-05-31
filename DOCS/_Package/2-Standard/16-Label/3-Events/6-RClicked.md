---
layout: default

grand_parent: Label Class
parent: Events
has_children: false
title: RClicked Event
nav_order: 6
permalink: /package/standard/label/events/rclicked
---
# {{ page.title }}

<br>

<br>
Occurs when the right mouse button is clicked.

 

The following child objects are attached to the Event object.

|  Type  | Name           | Description                                |
|:------:|----------------|--------------------------------------------|
| Number |  **ShiftKey**  | 1 if the Shift key is clicked, 0 otherwise |
| Number | **CtrlKey** | 1 if the Ctrl key is clicked, 0 otherwise  |
| Number |   **AltKey**   | 1 if the Alt key is clicked, 0 otherwise   |
| Number |    **xPos**    | X coordinate of mouse pointer              |
| Number |    **yPos**    | Y coordinate of mouse pointer              |

Example of use

```
Function OnRClicked(e) {
    MessageBox(strf("(%1,%2)で右クリックされました", e.xPos, e.yPos));
}
```
