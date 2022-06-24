---
layout: default

grand_parent: FlexView Class
parent: Events
has_children: false
title: FlexView.CursorMoved Event
nav_order: 1
permalink: /package/extension4/flexview/flexview/events/cursormoved
---
# {{ page.title }}

This event occurs when the cell cursor moves. The CursorMoved event has the following structure:

```
Event {
    FlexRow row; /* 移動した行をポイントするFlexRowオブジェクト */
    Number col; /* 移動した列番号 */
}
```

The cell cursor can be referenced by the RowPosition property and ColumnPosition property, but since the event goes through the event queue, the FlexRow object or col attached to the event caught by the event handler will have the cell cursor placed at that point. It may point to a different position than it is. Therefore, in order to manipulate the data of the cell in which the event occurred, be sure to specify the cell by the row and col attached to the event.

If you delete all rows or columns, the cell cursor moves to the invalid position. The row attached to the event that occurred at the invalid position is in the invalid state. Also, FlexView.InvalidPosition (-999) is set for col.