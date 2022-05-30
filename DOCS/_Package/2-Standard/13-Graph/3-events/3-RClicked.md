---
layout: default

grand_parent: Graph Class
parent: Events
has_children: false
title: RClicked Event
nav_order: 3
permalink: /package/standard/graph/events/rclicked
---
# {{ page.title }}

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
Function OnRClicked (e) {
    MessageBox (strf (" Right-clicked on (% 1,% 2) ", e.xPos, e.yPos));
}
```
