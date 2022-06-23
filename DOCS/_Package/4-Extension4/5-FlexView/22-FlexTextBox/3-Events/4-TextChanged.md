---
layout: default

grand_parent: FlexTextBox Class
parent: Events
has_children: false
title: FlexTextBox.TextChanged Event
nav_order: 4
permalink: /package/extension4/flexview/flextextbox/events/textchanged
---
# {{ page.title }}

This event occurs when the Value changes during the cell edit operation corresponding to the FlexTextBox. The TextChanged event has the following structure:

```
Event {
    FlexRow row; /* 移動した行をポイントするFlexRowオブジェクト */
}
```

The cell cursor can be referenced in the FlexView's RowPosition and ColumnPosition properties, but since the event goes through the event queue, the FlexRow object attached to the event caught by the event handler will have the cell cursor at that point. It may point to a line that is different from the position it is in. Therefore, in order to manipulate the data at the position where the event occurred, be sure to specify the row by the row of the event.