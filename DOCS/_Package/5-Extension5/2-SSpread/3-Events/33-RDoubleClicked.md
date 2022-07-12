---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.RDoubleClicked Event
nav_order: 33
permalink: /package/extension5/sspread/events/rdoubleclicked
---
# {{ page.title }}

Occurs when double-clicking the right mouse button on a cell.

The following child objects are attached to the Event object.

| Type   | Name           | Description                                                         |
|--------|----------------|---------------------------------------------------------------------|
| Number |    **_Col_**   | Column number of the cell where the right mouse button was clicked  |
| Number |    **_Row_**   | The row number of the cell where the right mouse button was clicked |
| Number | **_ShiftKey_** | 1 if the Shift key is pressed, 0 otherwise                          |
| Number |  **_CtrlKey_** | 1 if the Ctrl key is pressed, 0 otherwise                           |
| Number |  **_AltKey_**  | 1 if the Alt key is pressed, 0 otherwise                            |
| Number |   **_xPos_**   | X coordinate of mouse pointer                                       |
| Number |   **_yPos_**   | Y coordinate of mouse pointer                                       |

The event does not occur in the cell whose input mode is ON (edited state).

Example of usage<br>
```
Function OnRDoubleClicked (e) {
    MessageBox (strf ("(% 1,% 2) cell right mouse button was double-clicked ", e.Col, e.Row));
}
```

Related Item<br>
<a href="/package/extension5/sspread/events/clicked">Clicked</a>, <a href="/package/extension5/sspread/events/doubleclicked">DoubleClicked</a>, <a href="/package/extension5/sspread/events/lbuttonup">LButtonUp</a>, <a href="/package/extension5/sspread/events/rbuttonup">RButtonUp</a>, <a href="/package/extension5/sspread/events/rclicked">RClicked</a> event