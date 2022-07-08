---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.AfterLeaveCell Event
nav_order: 3
permalink: /package/extension5/sspread/events/afterleavecell
---
# {{ page.title }}

Occurs after moving the active cell.

The following child objects are attached to the Event object.

| Type   |     Name     | Description                   |
|--------|:------------:|-------------------------------|
| Number |   **_Col_**  | Active cell column number     |
| Number |   **_Row_**  | Active cell row number        |
| Number | **_NewCol_** | New active cell column number |
| Number | **_NewRow_** | New active cell row number    |

It also happens when the SSpread object loses focus. In this case, **_NewCol_** and  **_NewRow_** are -1.

This event does not occur if the <a href="/package/extension5/sspread/properties/operationmode">OperationMode</a> property is $OperationModeRead (read-only mode).

Also, if you move from the script, the event will not occur.
<br><small><span style="color:red">Added since Ver.5.0.2</span></small>

Example of usage

```
Function OnAfterLeaveCell(e) {
    if (e.NewCol < 0 || e.NewRow < 0) {
        return;
    }
    Col = e.Col;
    Row = e.Row;
    BackColor = $STD;
    Col = e.NewCol;
    Row = e.NewRow;
    BackColor = $RED;
}
```

Related Item<br>
<a href="/package/extension5/sspread/events/leavecell">LeaveCell</a> event

