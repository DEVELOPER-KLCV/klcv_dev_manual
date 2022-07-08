---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.DoubleClicked Event
nav_order: 20
permalink: /package/extension5/sspread/events/doubleclicked
---
# {{ page.title }}

Occurs when the left mouse button is double-clicked on a cell.

The following child objects are attached to the Event object.

| Type   |      Name      | Description                                                              |
|--------|:--------------:|--------------------------------------------------------------------------|
| Number |    **_Col_**   | Column number of the cell where the left mouse button was double-clicked |
| Number |    **_Row_**   | Row number of the cell where the left mouse button was double-clicked    |
| Number | **_ShiftKey_** | 1 if the Shift key is clicked, 0 otherwise                               |
| Number |  **_CtrlKey_** | 1 if the Ctrl key is clicked, 0 otherwise                                |
| Number |  **_AltKey_**  | 1 if the Alt key is clicked, 0 otherwise                                 |
| Number |   **_xPos_**   | X coordinate of mouse pointer                                            |
| Number |   **_yPos_**   | Y coordinate of mouse pointer                                            |

The event does not occur in the cell whose input mode is ON (edited state).

Example of usage<br>
```
Function OnDoubleClicked(e) {
    MessageBox (strf ("(% 1,% 2) cell was double-clicked ", e.Col, e.Row));
}
```

Related Item<br>
<a href="/package/extension5/sspread/events/clicked">Clicked</a>, <a href="/package/extension5/sspread/events/lbuttonup">LButtonUp</a>, <a href="/package/extension5/sspread/events/rbuttonup">RButtonUp</a>, <a href="/package/extension5/sspread/events/rdoubleclicked">RDoubleClicked</a> event 