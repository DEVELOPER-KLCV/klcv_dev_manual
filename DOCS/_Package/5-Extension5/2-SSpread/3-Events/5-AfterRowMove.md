---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.AfterRowMove Event
nav_order: 5
permalink: /package/extension5/sspread/events/afterrowmove
---
# {{ page.title }}

Occurs after the user moves a row by dragging and dropping.

The following child objects are attached to the Event object.

| Type   |      Name     | Description                         |
|--------|:-------------:|-------------------------------------|
| Number |   **_Row_**   | Row number of the row to move     |
| Number | **_RowDest_** | Row number of the destination row |

<small><span style="color:red">Added since Ver.5.0.2</span></small>

Example of usage

```
AllowRowMove = $TRUE;
Function OnAfterRowMove (e) {
    MessageBox (strf ("Moved from% 1st row to % 2nd row ", e.Row, e.RowDest));
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/allowrowmove">AllowRowMove</a> property<br>
<a href="/package/extension5/sspread/events/beforerowmove">BeforeRowMove</a> event

