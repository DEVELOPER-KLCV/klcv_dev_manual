---
layout: default

grand_parent: Spread Class
parent: Properties
has_children: false
title: Spread.LockColumns Property
nav_order: 16
permalink: /package/standard/spread/properties/lockcolumns
---
# {{ page.title }}
<br>

Specifies the number of columns to fix. Columns that are fixed are not subject to horizontal scrolling. <br>

You can specify a value from 0 to 32767 for the LockColumn property. 0 will unlock the column, and 1 will lock the leftmost column.<br>

Note that the value you specify is the number of columns on the display, not the column position of the <a href="/package/standard/spreadcolumn">SpreadColumn</a> object.<br><br>

Column-fixed columns behave similarly to row headers.

1. The <a href="/package/standard/spread/events/startedit">StartEdit</a> event does not occur

2. When pasting an editor object with the <a href="/package/standard/spread/events/startedit">StartEdit</a> method, the <a href="/package/standard/spread/methods/seteditor">SetEditor</a> event is immediately fired.

3. The column width cannot be changed with the mouse.

4. Even if the column is fixed to a column position that exceeds the Spread display range, the fixed column cannot be scrolled horizontally.