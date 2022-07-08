---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.AfterLeaveRow Event
nav_order: 4
permalink: /package/extension5/sspread/events/afterleaverow
---
# {{ page.title }}

Occurs after moving to another row with the OperationMode property $OperationModeRow (row mode).

The following child objects are attached to the Event object.

| Type   |          Name          | Description                                                                                     |
|--------|:----------------------:|-------------------------------------------------------------------------------------------------|
| Number |        **_Row_**       | Line number before moving                                                                       |
| Number |    **_RowWasLast_**    | $TRUE if the previous row is after the last row where the value is entered, $FALSE otherwise    |
| Number |    **_RowChanged_**    | $TRUE if the row value changes, $FALSE otherwise                                                |
| Number | **_AllCellsHaveData_** | $TRUE if all cells in the row are filled with values, $FALSE otherwise                          |
| Number |      **_NewRow_**      | Destination row number                                                                         |
| Number |   **_NewRowIsLast_**   | $TRUE if the destination row is after the last row where the value is entered, $FALSE otherwise |

The <a href="/package/extension5/sspread/events/enterrow">EnterRow</a> event is fired at the beginning of the row edit state.

If you move cells in the same row, the <a href="/package/extension5/sspread/events/leavecell">LeaveCell</a> and  <a href="/package/extension5/sspread/events/afterleavecell">AfterLeaveCell</a> events will occur.

If you move from the script, the event will not fire.

<small><span style="color:red">Added since Ver.5.0.2</span></small>

Example of usage

```
MaxCols = 5;
OperationMode = $OperationModeRow;
Function OnAfterLeaveRow(e) {
    Col = -1;
    Row = e.Row;
    BackColor = $STD;
    Row = e.NewRow;
    if (e.NewRowIsLast == $TRUE) {
        BackColor = $FFCCCC;
    } else {
        BackColor = $CCCCFF;
    }
    if (e.RowChanged == $TRUE) {
        Col = 0;
        Row = e.Row;
        if (e.AllCellsHaveData == $TRUE) {
            FontBold = $TRUE;
        } else {
            FontBold = $FALSE;
        }
        Col = -1;
        Row = e.Row;
        if (e.RowWasLast == $TRUE) {
            ForeColor = $RED;
        } else {
            ForeColor = $BLUE;
        }
    }
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/operationmode">OperationMode</a> property<br>
<a href="/package/extension5/sspread/events/enterrow">EnterRow</a>, <a href="/package/extension5/sspread/events/leaverow">LeaveRow</a> event