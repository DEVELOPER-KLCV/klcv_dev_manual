---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.ButtonClicked Event
nav_order: 12
permalink: /package/extension5/sspread/events/buttonclicked
---
# {{ page.title }}

Occurs when a button is clicked in a command button type and check box type cell.

The following child objects are attached to the Event object.

| Type   |       Name       | Description                                                                                                                                                                                                                                                  |
|--------|:----------------:|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Number |     **_Col_**    | Column number of the cell where the button was clicked                                                                                                                                                                                                       |
| Number |     **_Row_**    | Row number of the cell where the button was clicked                                                                                                                                                                                                          |
| Number | **_ButtonDown_** | Retained button (<a href="/package/extension5/sspread/properties/typebuttontype">TypeButtonType</a> property is $TypeButtonTypeTwoState) or checkbox state Retained button: $TRUE if pressed, $FALSE otherwise Buttons that are not retained buttons: Always $FALSE Checkbox: $TRUE if checked (or grayed out), $FALSE otherwise |

The event also occurs when you set the state of a retained button or check box from a CRS script using the <a href="/package/extension5/sspread/properties/type">Type</a>, <a href="/package/extension5/sspread/properties/value">Value</a> properties, and so on.

Example of usage <br>
```
Function OnButtonClicked (e) {
    Col = e.Col;
    Row = e.Row;
    if (CellType == $ CellTypeButton && TypeButtonType! = $ TypeButtonTypeTwoState) {
        MessageBox (strf ("(% 1,% 2) was pressed ", e.Col, e.Row));
    } else {
        if (e.ButtonDown == $ TRUE) {
            MessageBox (strf ("(% 1,% 2) checked ", e.Col, e.Row));
        } else {
            MessageBox (strf ("(% 1,% 2) unchecked ", e.Col, e.Row));
        }
    }
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/typebuttontype">TypeButtonType</a>, <a href="/package/extension5/sspread/properties/value">Value</a> property

