---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.AfterColMove Event
nav_order: 2
permalink: /package/extension5/sspread/events/aftercolmove
---
# {{ page.title }}

Occurs after the user moves a column by dragging and dropping.

The following child objects are attached to the Event object.

| Type   |      Name     | Description                             |
|--------|:-------------:|-----------------------------------------|
| Number |   **_Col_**   | Column number of the column to move     |
| Number | **_ColDest_** | Column number of the destination column |

<small><span style="color:red">Added since Ver.5.0.2</span></small>

Example of usage

```
AllowColMove = $TRUE;
Function OnAfterColMove(e) {
    MessageBox(strf("Moved from % 1st column to % 2nd column", e.Col, e.ColDest));
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/allowcolmove">AllowColMove</a> property, <a href="/package/extension5/sspread/events/beforecolmove">BeforeColMove</a> event



 
