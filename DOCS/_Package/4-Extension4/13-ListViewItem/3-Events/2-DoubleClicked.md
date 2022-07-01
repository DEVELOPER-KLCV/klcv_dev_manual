---
layout: default

grand_parent: ListViewItem Class
parent: Events
has_children: false
title: ListViewItem.DoubleClicked Event
nav_order: 2
permalink: /package/extension4/listviewitem/events/doubleclicked
---
# {{ page.title }}

Occurs when you double-click an item.

The following child objects are attached to the Event object.

| Type   |     Name     | Description                                |
|--------|:------------:|--------------------------------------------|
| Number | **_ShiftKey_** | 1 if the Shift key is clicked, 0 otherwise |
| Number |  **_CtrlKey_** | 1 if the Ctrl key is clicked, 0 otherwise  |
| Number |  **_AltKey_**  | 1 if the Alt key is clicked, 0 otherwise   |
| Number |   **_xPos_**   | X coordinate of mouse pointer              |
| Number |   **_yPos_**   | Y coordinate of mouse pointer              |

<a href="/package/extension4/listviewitem/events/#precautions-when-referring-to-selection-items">Precautions when referring to selection items</a>