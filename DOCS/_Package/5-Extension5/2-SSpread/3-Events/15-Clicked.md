---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.Clicked Event
nav_order: 15
permalink: /package/extension5/sspread/events/clicked
---
# {{ page.title }}

Occurs when the left mouse button is clicked on a cell.

The following child objects are attached to the Event object.

| Type   |       Name       | Description                                                        |
|--------|:----------------:|--------------------------------------------------------------------|
| Number |     **_Col_**    | Column number of the cell where the left mouse button was clicked  |
| Number |     **_Row_**    | The row number of the cell where the left mouse button was clicked |
| Number |  **_ShiftKey_**  | 1 if the Shift key is clicked, 0 otherwise                         |
| Number | **_CtrlKeyKey_** | 1 if the Ctrl key is clicked, 0 otherwise                          |
| Number |   **_AltKey_**   | 1 if the Alt key is clicked, 0 otherwise                           |
| Number |    **_xPos_**    | X coordinate of mouse pointer                                      |
| Number |    **_yPos_**    | Y coordinate of mouse pointer                                      |

If the <a href="/package/extension5/sspread/properties/moveactiveonfocus">MoveActiveOnFocus</a> property is $FALSE, no event will be fired when the spreadsheet is clicked and focused.

The event does not occur in the cell whose input mode is ON (edited state).

Example of usage <br>
```
Function OnClicked (e) {
    MessageBox (strf ("(% 1,% 2) cell was clicked ", e.Col, e.Row));
}
```

Related Item<br>
<a href="/package/extension5/sspread/events/doubleclicked">DoubleClicked</a>, <a href="/package/extension5/sspread/events/lbuttonup">LButtonUp</a>, <a href="/package/extension5/sspread/events/rbutoonup">RButtonUp</a>, <a href="/package/extension5/sspread/events/rclicked">RClicked</a>, <a href="/package/extension5/sspread/events/rdoubleclicked">RDoubleClicked</a> event