---
layout: default

grand_parent: TrayIcon Class
parent: Events
has_children: false
title: DoubleClicked Event
nav_order: 2
permalink: /package/extension4/trayicon/events/doubleclicked
---
# {{ page.title }}

Occurs when the left mouse button is double-clicked.

The following child objects are attached to the Event object.

| Type   |     Name     | Description                                |
|--------|:------------:|--------------------------------------------|
| Number | **_ShiftKey_** | 1 if the Shift key is clicked, 0 otherwise |
| Number |  **_CtrlKey_** | 1 if the Ctrl key is clicked, 0 otherwise  |
| Number |  **_AltKey_**  | 1 if the Alt key is clicked, 0 otherwise   |
| Number |   **_xPos_**   | X coordinate of mouse pointer              |
| Number |   **_yPos_**   | Y coordinate of mouse pointer              |


Usage example

```
Function OnDoubleClicked(e) {
    MessageBox(strf("(%1,%2)でダブルクリックされました", e.xPos, e.yPos));
}
```