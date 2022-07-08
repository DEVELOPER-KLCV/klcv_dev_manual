---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.ComboSelChange Event
nav_order: 19
permalink: /package/extension5/sspread/events/comboselchange
---
# {{ page.title }}

Occurs when the user changes the selection of a combo box cell.

The following child objects are attached to the Event object.

| Type   |    Name   | Description                       |
|--------|:---------:|-----------------------------------|
| Number | **_Col_** | Column number of combo box type cell      |
| Number | **_Row_** | Row number of combo box type cell |

When the drop-down list is open, the event also fires when you change the selection with the direction keys.

Example of usage

```
Function OnComboSelChange(e) {
    Col = e.Col;
    Row = e.Row;
    TypeComboBoxIndex = TypeComboBoxCurSel;
    print(TypeComboBoxString, "\n");
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> property<br>
<a href="/package/extension5/sspread/events/combocloseup">ComboCloseUp</a>, <a href="/package/extension5/sspread/events/combodropdown">ComboDropDown</a> event
