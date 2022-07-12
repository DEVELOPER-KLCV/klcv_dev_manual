---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.RowHeightChange Event
nav_order: 34
permalink: /package/extension5/sspread/events/rowheightchange
---
# {{ page.title }}

Occurs when changing the row height with the mouse.

The following child objects are attached to the Event object.

| Type   | Name       | Description                                     |
|--------|------------|-------------------------------------------------|
| Number | **_Row1_** | The first row number in the changed row range |
| Number | **_Row2_** | The last row number in the changed row range  |

Example of usage <br>
```
Function OnRowHeightChange (e) {
    for (var r = e.Row1; r <= e.Row2; r ++) {
        if (RowHeight (r)> 40) {
            RowHeight (r) = 40;
        }
    }
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/rowheight">RowHeight</a>, <a href="/package/extension5/sspread/properties/userresize">UserResize</a>, <a href="/package/extension5/sspread/properties/userresizerow">UserResizeRow</a> property<br>
<a href="/package/extension5/sspread/events/colwidthchange">ColWidthChange</a> event