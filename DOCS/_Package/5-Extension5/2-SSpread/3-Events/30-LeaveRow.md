---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.LeaveRow Event
nav_order: 30
permalink: /package/extension5/sspread/events/leaverow
---
# {{ page.title }}

Occurs before moving to another row with the <a href="/package/extension5/sspread/properties/operationmode">OperationMode</a> property $OperationModeRow (row mode).

※ The move is not complete when this event occurs. Use the <a href="/package/extension5/sspread/events/afterleaverow">AfterLeaveRow</a> event when performing processing that is expected to be completed after the move is completed.

The following child objects are attached to the Event object.

| Type   | Name                   | Description                                                                                     |
|--------|------------------------|-------------------------------------------------------------------------------------------------|
| Number |        **_Row_**       | Row number before moving                                                                        |
| Number |    **_RowWasLast_**    | $TRUE if the previous row is after the last row where the value is entered , otherwise $FALSE   |
| Number |    **_RowChanged_**    | $TRUE if the row value changes, $FALSE otherwise                                                |
| Number | **_AllCellsHaveData_** | $TRUE if all cells in the row are populated, $FALSE otherwise                                   |
| Number |      **_NewRow_**      | Destination row number                                                                          |
| Number |   **_NewRowIsLast_**   | $TRUE if the destination row is after the last row where the value is entered, $FALSE otherwise |


The EnterRow event is fired at the beginning of the row edit state.

If move cells in the same row, the LeaveCell and AfterLeaveCell events will occur.

If move from the script, the event will not fire.

Example of usage<br>
```
MaxCols = 5;
OperationMode = $OperationModeRow;
Function OnLeaveRow(e) {
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
<a href="/package/extension5/sspread/events/afterleaverow">AfterLeaveRow</a>, <a href="/package/extension5/sspread/enterrow">EnterRow</a> event 





