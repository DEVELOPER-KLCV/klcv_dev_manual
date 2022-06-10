---
layout: default

grand_parent: Spread Class
parent: Events
has_children: false
title: Spread.StopEdit Event
nav_order: 7
permalink: /package/standard/spread/events/stopedit
---
# {{ page.title }}
<br>
Occurs when the edit window is disabled.

 

The following child objects are attached to the Event object.

|  Type  |    Name   | Description                                       |
|:------:|:---------:|---------------------------------------------------|
| Number | **_row_** | Row position where the edit window is disabled    |
| Number | **_col_** | Column position where the edit window is disabled |

The **_row_** and **_col_** are set to the row and column numbers that were previously in the edit state.

<br><small><span style="color:red">Since Ver.4.0.2, Spread.InvalidPosition is set for row and col set in the StopEdit event that occurs when the row being edited is deleted.</span></small>

Example
```
Number edit_row;
Number edit_col;
Function OnStopEdit(e) {
    var edit = null;
    var col = e.col;
    if (col == Spread.InvalidPosition) {
        col = edit_col;
    }
    switch (col) {
    case 0:
        edit = frmSpreadEdit.ebText;
        break;
    case 1:
        edit = frmSpreadEdit.ebNumber;
        break;
    case 2:
        edit = frmSpreadEdit.ebDate;
        break;
    default:
        edit_row = -1;
        edit_col = -1;
        return;
    }
    if (edit_row == e.row && edit_col == e.col) {
        SetCell(e.row, e.col, edit.Value);
    }
    if (edit != null) {
        edit.Visible = $FALSE;
    }
    edit_row = -1;
    edit_col = -1;
}
```

Since Biz / Browser events go through the event queue, be sure to use the row and col objects that are passed as child objects of the <a href="/package/standard/spread/events/startedit">StartEdit</a>  event or StopEdit event. In the OnStartEdit, OnStopEdit event handler, if you use the <a href="/package/standard/spread/properties/value">Value</a> and <a href="/package/standard/spread/properties/columnposition">ColumnPosition</a> properties to get the cursor position, it may be different from the position notified by the event.<br><br>

 

The  <a href="/package/standard/spread/events/startedit">StartEdit</a> event is paired with the StopEdit event, but there is no guarantee of its order of occurrence. Note that the following events can occur:
```
StartEdit (row=0, col=0)
StartEdit (row=1, col=0)
StopEdit  (row=0, col=0)
StopEdit  (row=1, col=0)
```
