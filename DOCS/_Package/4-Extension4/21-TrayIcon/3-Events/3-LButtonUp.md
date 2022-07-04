---
layout: default

grand_parent: TrayIcon Class
parent: Events
has_children: false
title: LButtonUp Event
nav_order: 3
permalink: /package/extension4/trayicon/events/lbuttonup
---
# {{ page.title }}

Occurs when the left mouse button is released.

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
Function OnLButtonUp(e) {
    MessageBox(strf("(%1,%2)でマウス左ボタンが離されました", e.xPos, e.yPos));
}
```