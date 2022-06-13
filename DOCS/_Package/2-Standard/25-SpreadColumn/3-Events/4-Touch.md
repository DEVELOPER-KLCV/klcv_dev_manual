---
layout: default

grand_parent: SpreadColumn Class
parent: Events
has_children: false
title: SpreadColumn.Touch Event
nav_order: 4
permalink: /package/standard/spreadcolumn/events/touch
---
# {{ page.title }}
<br>

This event occurs when you select a cell.
It occurs regardless of the operation from the screen or the operation from the script.

***Note***<br>
In the handler of the event that occurred in the SpreadColumn class, do not use the <a href="/package/standard/spread/properties/value">Value</a> and  <a href="/package/standard/spreadcolumn/events/columnposition">ColumnPosition</a> properties of the parent object  <a href="/package/standard/spread">Spread</a> class to refer to the current cursor position. (The cursor position may not be reflected.)

For the column position, refer to the From property (SpreadColumn object) of the Event object passed as an argument of the event handler, and for the row position, refer to the Index property (array subscript) of the parent object of the From property (SpreadRow object, which can be referenced by From. ^).

