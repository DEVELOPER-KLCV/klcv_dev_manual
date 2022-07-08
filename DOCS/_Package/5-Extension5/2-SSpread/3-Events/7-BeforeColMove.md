---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.BeforeColMove Event
nav_order: 7
permalink: /package/extension5/sspread/events/beforecolmove
---
# {{ page.title }}

Occurs when the user tries to move a column by dragging and dropping.

※ The movement of the column has not been completed when this event occurs. Use the AfterColMove event if you want to perform processing that is expected after the column has been moved.

The following child objects are attached to the Event object.

| Type   |      Name     | Description                             |
|--------|:-------------:|-----------------------------------------|
| Number |   **_Col_**   | Column number of the column to move     |
| Number | **_ColDest_** | Column number of the destination column |

Example of usage

```
AllowColMove = $TRUE;
Function OnBeforeColMove (e) {
    MessageBox ( strf ("Move from% 1st column to % 2nd column ", e.Col , e.ColDest ));
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/allocolmove">AllowColMove</a> property<br>
<a href="/package/extension5/sspread/events/aftercolmove">AfterColMove</a> event





