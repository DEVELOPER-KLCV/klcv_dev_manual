---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.EnterRow Event
nav_order: 27
permalink: /package/extension5/sspread/events/enterrow
---
# {{ page.title }}

Occurs when the <a href="/package/extension5/sspread/properties/operationmode">OperationMode</a> property is $OperationModeRow (row mode), go to a new row and double-click (when in row edit state).

The following child objects are attached to the Event object.

| Type   | Name            | Description                                                                    |
|--------|-----------------|--------------------------------------------------------------------------------|
| Number |    **_Row_**    | Destination row number                                                         |
| Number | **_RowIsLast_** | $TRUE for rows after the last row where the value is entered, $FALSE otherwise |

The <a href="/package/extension5/sspread/events/leaverow">LeaveRow</a> event is fired when the row edit state ends.

Example of usage <br>
```
OperationMode = $OperationModeRow;
Function OnEnterRow(e) {
    Col = -1;
    Row = e.Row;
    if (e.RowIsLast == $TRUE) {
        BackColor = $CCFFFF;
    } else {
        BackColor = $FFFFCC;
    }
}
```

Related Items <br>
<a href="/package/extension5/sspread/properties/operationmode">OperationMode</a> property<br> <a href="/package/extension5/sspread/events/editmodeon">EditModeOn</a>, <a href="/package/extension5/sspread/events/leaverow">LeaveRow</a> event