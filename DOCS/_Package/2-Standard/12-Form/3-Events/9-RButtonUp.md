---
layout: default

grand_parent: Form Class
parent: Events
has_children: false
title: RButtonUp Event
nav_order: 9
permalink: /package/standard/form/events/rbuttonup
---
# {{ page.title }}

<br>

Occurs when the right mouse button is released.

 

The following child objects are attached to the Event object.

|  Type  |      Name      | Description                                |
|:------:|:--------------:|--------------------------------------------|
| Number |  **ShiftKey**  | 1 if the Shift key is pressed, 0 otherwise |
| Number | **CtrlKeyKey** | 1 if the Ctrl key is pressed, 0 otherwise  |
| Number |   **AltKey**   | 1 if the Alt key is pressed, 0 otherwise   |
| Number |    **xPos**    | X coordinate of mouse pointer              |
| Number |    **yPos**    | Y coordinate of mouse pointer              |

<br><small><span style="color:red">Added since Ver.4.1.0</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>

Example of use

```
Function OnRButtonUp(e) {
    MessageBox(strf("(%1,%2)でマウス右ボタンが離されました", e.xPos, e.yPos));
}
```

