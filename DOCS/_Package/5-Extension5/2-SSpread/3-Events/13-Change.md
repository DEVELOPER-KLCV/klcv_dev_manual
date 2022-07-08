---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.Change Event
nav_order: 13
permalink: /package/extension5/sspread/events/change
---
# {{ page.title }}

Occurs when the value of the active cell is changed and when the value of the cell referenced in the formula is changed.

The following child objects are attached to the Event object.

| Type   |    Name   | Description                                       |
|--------|:---------:|---------------------------------------------------|
| Number | **_Col_** | Column number of the cell whose value has changed |
| Number | **_Row_** | Row number of the cell whose value has changed    |

When the value of the cell referenced in the formula changes, the event is fired for all related cells.

In the event handler for this event, the Text and Value properties can be used to get the value of the modified cell.

If change the value from the script, the event will not fire.

Example of usage<br>
```
Function OnChange(e) {
    Col = e.Col;
    Row = e.Row;
    if (Text == "") {
        BackColor = $RED;
    }
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/value">Value</a> property