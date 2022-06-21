---
layout: default

grand_parent: FlexHeader Class
parent: Events
has_children: false
title: FlexHeader.RClicked Events
nav_order: 3
permalink: /package/extension4/flexview/flexheader/events/rclicked
---
# {{ page.title }}

This is an event that occurs when you right-click on the cell corresponding to FlexHeader.

The RClicked event has the following structure:

```
Event {
    FlexRow row; /* 移動した行をポイントするFlexRowオブジェクト */
}
```

The cell cursor can be referenced in the FlexView's RowPosition and ColumnPosition properties, but since the event goes through the event queue, the FlexRow object attached to the event caught by the event handler will have the cell cursor at that point. It may point to a row that is different from the position it is in. Therefore, in order to manipulate the data at the position where the event occurred, be sure to specify the row by the row of the event.