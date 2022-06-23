---
layout: default

grand_parent: FlexTextBox Class
parent: Events
has_children: false
title: FlexTextBox.BeginEdit Event
nav_order: 1
permalink: /package/extension4/flexview/flextextbox/events/beginedit
---
# {{ page.title }}

This event occurs when you start editing the FlexTextBox.

The BeginEdit event has the following structure:

```
Event {
    FlexRow row; /* 発生した行をポイントするFlexRowオブジェクト */
}
```

The cell cursor can be referenced in the FlexView's RowPosition and ColumnPosition properties, but since the event goes through the event queue, the FlexRow object attached to the event caught by the event handler will have the cell cursor at that point. It may point to a line that is different from the position it is in. Therefore, in order to manipulate the data at the position where the event occurred, be sure to specify the row by the row of the event.

<br><small><span style="color:red">Added since Ver.5.1.0</span></small>