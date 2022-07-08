---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.ColWidthChange Event
nav_order: 16
permalink: /package/extension5/sspread/events/colwidthchange
---
# {{ page.title }}

Occurs when changing the width of a column with the mouse.

The following child objects are attached to the Event object.

| Type   |    Name    | Description                                             |
|--------|:----------:|---------------------------------------------------------|
| Number | **_Col1_** | The leftmost column number of the changed column range  |
| Number | **_Col2_** | The rightmost column number of the changed column range |

Example of usage<br>
```
Function OnColWidthChange(e) {
    for (var c = e.Col1; c <= e.Col2; c++) {
        if (ColWidth(c) > 100) {
            ColWidth(c) = 100;
        }
    }
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/colwidth">ColWidth</a>, <a href="/package/extension5/sspread/properties/userresize">UserResize</a>,  <a href="/package/extension5/sspread/properties/userresizecol">UserResizeCol</a> property<br> <a href="/package/extension5/sspread/events/rowheightchange">RowHeightChange</a> event