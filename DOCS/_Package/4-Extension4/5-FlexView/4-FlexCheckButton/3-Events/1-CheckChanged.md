---
layout: default

grand_parent: FlexCheckButton Class
parent: Events
has_children: false
title: FlexCheckButton.CheckChanged Event
nav_order: 1
permalink: /package/extension4/flexview/flexcheckbutton/events/checkchanged
---
# {{ page.title }}

This event occurs when the check state of the cell corresponding to FlexCheckButton is changed. The CheckChanged event has the following structure:

```
Event {
    FlexRow row; /* 移動した行をポイントするFlexRowオブジェクト */
}
```

The cell cursor can be referenced in the FlexView's RowPosition and ColumnPosition properties, but since the event goes through the event queue, the FlexRow object attached to the event caught by the event handler will have the cell cursor at that point. It may point to a row that is different from the position it is in. Therefore, in order to manipulate the data at the position where the event occurred, be sure to specify the row by the row of the event.