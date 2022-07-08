---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.ComboCloseUp Event
nav_order: 17
permalink: /package/extension5/sspread/events/combocloseup
---
# {{ page.title }}

Occurs when the drop-down list of combo box cells is closed.

The following child objects are attached to the Event object.

| Type   |       Name      | Description                                                                       |
|--------|:---------------:|-----------------------------------------------------------------------------------|
| Number |    **_Col_**    | Combo box cell column number                                                      |
| Number |    **_Row_**    | Row number of combo box type cell                                                 |
| Number | **_SelChange_** | Index of items selected when closed <br> -1 if the same item as last time was selected |

The timing of the occurrence of this event and the determination of the cell value are different. The <a href="/package/extension5/sspread/events/change">Change</a> event is fired when the cell value change is confirmed, and the <a href="/package/extension5/sspread/events/editmodeoff">EditModeOff</a> event is fired when the cell editing is complete.

SelChange is set to the item that was selected when it was closed, not the confirmed item. Even if you cancel with the ESC key, the item selected at that time will be set.

Check the selected value in the Change and EditModeOff events.

Example of usage<br>
```
Function OnComboCloseUp(e) {
    if (e.SelChange >= 0) {
        Col = e.Col;
        Row = e.Row;
        TypeComboBoxIndex = e.SelChange;
        MessageBox(TypeComboBoxString + "が選択されました");
    }
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> property<br>
<a href="/package/extension5/sspread/events/change">Change</a>,  <a href="/package/extension5/sspread/events/combodropdown">ComboDropDown</a>, <a href="/package/extension5/sspread/events/comboselchange">ComboSelChange</a>, <a href="/package/extension5/sspread/events/editmodeoff">EditModeOff</a> event