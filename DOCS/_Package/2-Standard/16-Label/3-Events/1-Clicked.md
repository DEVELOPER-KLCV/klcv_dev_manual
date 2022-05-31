---
layout: default

grand_parent: Label Class
parent: Events
has_children: false
title: Clicked Event
nav_order: 1
permalink: /package/standard/label/events/clicked
---
# {{ page.title }}

<br>
Occurs when the left mouse button is clicked.

 

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
Function OnClicked(e) {
    MessageBox(strf("(%1,%2)でクリックされました", e.xPos, e.yPos));
}
```