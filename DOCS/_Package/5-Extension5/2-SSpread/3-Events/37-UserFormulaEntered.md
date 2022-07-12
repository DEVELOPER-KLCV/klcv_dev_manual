---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.UserFormulaEntered Event
nav_order: 37
permalink: /package/extension5/sspread/events/userformulaentered
---
# {{ page.title }}

Occurs when <a href="/package/extension5/sspread/properties/allowuserformulas">AllowUserFormulas</a> is set to $TRUE and the user enters a formula in a cell.

The following child objects are attached to the Event object.

| Type   | Name      | Description                                  |
|--------|-----------|----------------------------------------------|
| Number | **_Col_** | Column number of the entered or changed cell |
| Number | **_Row_** | Row number of cell entered or changed        |

Example of usage<br>
```
AllowUserFormulas = $TRUE;
Function OnUserFormulaEntered(e) {
    Col = e.Col;
    Row = e.Row;
    MessageBox (strf ("(% 1,% 2) cell formula changed to % 3 ", Col, Row, Formula));
}
```

Related Item
<a href="/package/extension5/sspread/properties/allowuserformulas">AllowUserFormulas</a>, <a href="/package/extension5/sspread/properties/formula">Formula</a> property 