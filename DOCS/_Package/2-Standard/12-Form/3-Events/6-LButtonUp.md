---
layout: default

grand_parent: Form Class
parent: Events
has_children: false
title: LButtonUp Event
nav_order: 6
permalink: /package/standard/form/events/lbuttonup
---
# {{ page.title }}

<br>

Occurs when the left mouse button is released.

 

The following child objects are attached to the Event object.


| Type   | Name       | Description                                |
|:--------:|:--------------:|--------------------------------------------|
| Number |  **ShiftKey**  | 1 if the Shift key is pressed, 0 otherwise |
| Number | **CtrlKeyKey** | 1 if the Ctrl key is pressed, 0 otherwise  |
| Number |   **AltKey**   | 1 if the Alt key is pressed, 0 otherwise   |
| Number |    **xPos**    | X coordinate of mouse pointer              |
| Number |    **yPos**    | Y coordinate of mouse pointer              |



<br><small><span style="color:red">Added since Ver.4.1.0</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>

<br>

Example of use

```
Function OnLButtonUp (e) {
    MessageBox (strf ("(% 1,% 2) released mouse left button ", e.xPos, e.yPos));
}
```

