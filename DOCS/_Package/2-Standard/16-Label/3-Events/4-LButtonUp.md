---
layout: default

grand_parent: Label Class
parent: Events
has_children: false
title: LButtonUp Event
nav_order: 4
permalink: /package/standard/label/events/lbuttonup
---
# {{ page.title }}

<br>
Occurs when the left mouse button is released.

 

The following child objects are attached to the Event object.

|  Type  | Name           | Description                                |
|:------:|----------------|--------------------------------------------|
| Number |  **ShiftKey**  | 1 if the Shift key is clicked, 0 otherwise |
| Number | **CtrlKey** | 1 if the Ctrl key is clicked, 0 otherwise  |
| Number |   **AltKey**   | 1 if the Alt key is clicked, 0 otherwise   |
| Number |    **xPos**    | X coordinate of mouse pointer              |
| Number |    **yPos**    | Y coordinate of mouse pointer              |

<br><small><span style="color:red">Added since Ver.4.1.0</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>

Example of use

```
Function OnLButtonUp(e) {
    MessageBox(strf("(%1,%2)でマウス左ボタンが離されました", e.xPos, e.yPos));
}
```
