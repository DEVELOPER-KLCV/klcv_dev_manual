---
layout: default

grand_parent: SpreadColumn Class
parent: Events
has_children: false
title: SpreadColumn.RClicked Event
nav_order: 3
permalink: /package/standard/spreadcolumn/events/rclicked
---
# {{ page.title }}
<br>

This event occurs when you right-click a cell. If no lines are displayed, the RClicked event will not be fired.

The following child objects are attached to the Event object.

| Type   | Name           | Description                                |
|--------|----------------|--------------------------------------------|
| Number | **_ShiftKey_** | 1 if the Shift key is pressed, 0 otherwise |
| Number | **_CtrlKey_**  | 1 if the Ctrl key is pressed, 0 otherwise  |
| Number | **_AltKey_**   | 1 if the Alt key is pressed, 0 otherwise   |
| Number | **_xPos_**     | X coordinate of mouse pointer              |
| Number | **_yPos_**     | Y coordinate of mouse pointer              |
| Number | **_row_**      | Row position of the clicked cell           |
| Number | **_col_**      | Column position of clicked cell            |


***Notes***

In the handler of the event that occurred in the SpreadColumn class, do not use the <a href="/package/standard/spread/properties/value">Value</a> and <a href="/package/standard/spreadcolumn/events/columnposition">ColumnPosition</a> properties of the parent object <a href="/package/standard/spread">Spread</a> class to refer to the current cursor position. (The cursor position may not be reflected.)

To refer to the cell position that was right-clicked, use the ***row*** and ***col*** passed as the argument of the event handler.