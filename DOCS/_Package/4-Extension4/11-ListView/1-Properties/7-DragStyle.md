---
layout: default

grand_parent: ListView Class
parent: Properties
has_children: false
title: ListView.DragStyle Property
nav_order: 7
permalink: /package/extension4/listview/properties/dragstyle
---
# {{ page.title }}

The behavior of the icon. Only valid for ListStyle of $LARGEICON or $SMALLICON.

| Constant   | Value |  Description  |
|:----------:|:-----:|:-------------:|
| $STD       |   0   |   Cannot move |
| $MOVE      |   1   |   Draggable   |


With DragStyle = $MOVE, the position is only temporarily changed, and the internal value does not change at all.

<br><small><span style="color:green">It has been changed to the following specifications since Ver.4.1.3</span></small>

DragStyle = $ MOVE inserts the additional line at the end, and $ STD inserts it in the appropriate position in ascending order.

If you change the ListStyle to something other than $LARGEICON or $SMALLICON and then return it again, it will be displayed again in ascending order.