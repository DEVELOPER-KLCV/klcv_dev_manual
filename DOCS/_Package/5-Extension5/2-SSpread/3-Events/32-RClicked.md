---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.RClicked Event
nav_order: 32
permalink: /package/extension5/sspread/events/rclicked
---
# {{ page.title }}

Occurs when the right mouse button is pressed on a cell.

The following child objects are attached to the Event object.

| Type   | Name             | Description                                                         |
|--------|------------------|---------------------------------------------------------------------|
| Number |     **_Col_**    | Column number of the cell where the right mouse button was clicked  |
| Number |     **_Row_**    | The row number of the cell where the right mouse button was clicked |
| Number |  **_ShiftKey_**  | 1 if the Shift key is pressed, 0 otherwise                          |
| Number | **_CtrlKey_** | 1 if the Ctrl key is pressed, 0 otherwise                           |
| Number |   **_AltKey_**   | 1 if the Alt key is pressed, 0 otherwise                            |
| Number |    **_xPos_**    | X coordinate of mouse pointer                                       |
| Number |    **_yPos_**    | Y coordinate of mouse pointer                                       |

The event does not occur in the cell whose input mode is ON (edited state).

Example of usage <br>
```
Function OnRClicked (e) {
    MessageBox (strf (" Right clicked on cell (% 1,% 2) ", e.Col, e.Row));
}
```

Related Item<br>
<a href="/package/extension5/sspread/events/clicked">Clicked</a>, <a href="/package/extension5/sspread/events/doubleclicked">DoubleClicked</a>, <a href="/package/extension5/sspread/events/lbuttonup">LButtonUp</a>, <a href="/package/extension5/sspread/events/rbuttonup">RButtonUp</a>, <a href="/package/extension5/sspread/events/rdoubleclicked">RDoubleClicked</a> event