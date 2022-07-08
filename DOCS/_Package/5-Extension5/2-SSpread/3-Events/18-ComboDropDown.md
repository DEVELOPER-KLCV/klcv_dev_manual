---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.ComboDropDown Event
nav_order: 18
permalink: /package/extension5/sspread/events/combodropdown
---
# {{ page.title }}

Occurs when the drop-down list of combo box cells is opened.

The following child objects are attached to the Event object.

| Type   |    Name   | Description                       |
|--------|:---------:|-----------------------------------|
| Number | **_Col_** | Combo box cell column number      |
| Number | **_Row_** | Row number of combo box type cell |

The drop-down list opens when you click the arrow button to the right of the combo box cell or when you press the bottom of the Alt + Direction key.

Example of usage

```
Function OnComboDropDown(e) {
    print(e.Col, e.Row, "\n");
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> property<br>
<a href="/package/extension5/sspread/events/combocloseup">ComboCloseUp</a>, <a href="/package/extension5/sspread/events/comboselchange">ComboSelChange</a> event

