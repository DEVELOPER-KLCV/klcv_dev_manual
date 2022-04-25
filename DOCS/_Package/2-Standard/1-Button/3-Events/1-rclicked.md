---
layout: default

grand_parent: Button Class
parent: Events
has_children: false
title: RClicked Event
nav_order: 1
permalink: /package/standard/button/events/rclicked
---
# {{ page.title }}

Occurs when the right mouse button is pressed.

The following child objects are attached to the Event object.

| Type  | Name       | Description |
|-------|------------|-------------|
|Number |**ShiftKey**|1 if the Shift key is pressed, 0 otherwise |
|Number |**CtrlKey**|1 if the Ctrl key is pressed, 0 otherwise |
|Number |**AltKey**|1 if the Alt key is pressed, 0 otherwise |
|Number |**xPos**|X coordinate of mouse pointer |
|Number |**yPos**|Y coordinate of mouse pointer |

Use Case

```
Function OnRClicked(e) {
    MessageBox(strf("Right clicked at point (%1,%2)", e.xPos, e.yPos));
}
```




