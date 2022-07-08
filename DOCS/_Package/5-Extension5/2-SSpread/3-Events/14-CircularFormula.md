---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.CircularFormula Event
nav_order: 14
permalink: /package/extension5/sspread/events/circularformula
---
# {{ page.title }}

Occurs when a circular reference is used when recalculating a formula.

The following child objects are attached to the Event object.

| Type   |    Name   | Description                                       |
|--------|:---------:|---------------------------------------------------|
| Number | **_Col_** | Column number of the cell whose value has changed |
| Number | **_Row_** | Row number of the cell whose value has changed    |

Example of usage<br>
```
Function OnCircularFormula(e) {
    MessageBox (strf ("(% 1,% 2) cells are circularly referenced ", e.Col, e.Row));
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/allowuserformulas">AllowUserFormulas</a>, <a href="/package/extension5/sspread/properties/formula">Formula</a> property