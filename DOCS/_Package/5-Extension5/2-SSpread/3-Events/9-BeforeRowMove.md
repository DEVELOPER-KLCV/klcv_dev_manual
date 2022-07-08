---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.BeforeRowMove Event
nav_order: 9
permalink: /package/extension5/sspread/events/beforerowmove
---
# {{ page.title }}

Occurs when the user tries to move a row by dragging and dropping.

※ Line movement has not been completed when this event occurs. Use the AfterRowMove event if you want to perform processing that is expected after the row has been moved.

The following child objects are attached to the Event object.

| Type   |      Name     | Description                       |
|--------|:-------------:|-----------------------------------|
| Number |   **_Row_**   | Row number of the row to move     |
| Number | **_RowDest_** | Row number of the destination row |

Example of usage

```
AllowRowMove = $TRUE;
Function OnBeforeRowMove (e) {
    MessageBox ( strf ("Move from% 1st row to % 2nd row ", e.Row , e.RowDest ));
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/allowrowmove">AllowRowMove</a> property <br> <a href="/package/extension5/sspread/events/afterrowmove">AfterRowMove</a> event


