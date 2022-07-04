---
layout: default

grand_parent: TrayIcon Class
parent: Events
has_children: false
title: RButtonUp Event
nav_order: 4
permalink: /package/extension4/trayicon/events/rbuttonup
---
# {{ page.title }}

Occurs when the right mouse button is released.

The following child objects are attached to the Event object.

| Type   |     Name     | Description                                |
|--------|:------------:|--------------------------------------------|
| Number | **_ShiftKey_** | 1 if the Shift key is clicked, 0 otherwise |
| Number |  **_CtrlKey_** | 1 if the Ctrl key is clicked, 0 otherwise  |
| Number |  **_AltKey_**  | 1 if the Alt key is clicked, 0 otherwise   |
| Number |   **_xPos_**   | X coordinate of mouse pointer              |
| Number |   **_yPos_**   | Y coordinate of mouse pointer              |

<small><span style="color:red">Added since Ver.4.1.0</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>

Usage example

```
Function OnRButtonUp(e) {
    MessageBox(strf("(%1,%2)でマウス右ボタンが離されました", e.xPos, e.yPos));
}
```