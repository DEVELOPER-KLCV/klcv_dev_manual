---
layout: default

grand_parent: StyleEdit Class
parent: Properties
has_children: false
title: StyleEdit.LineWidthLimit Property
nav_order: 12
permalink: /package/extension4/styleedit/properties/linewidthlimit
---
# {{ page.title }}

This property is valid only when WordWrap = $TRUE.

A value from 0 or 10 to 1000 can be specified, and if 0 is specified, the line width will be the display size. If a value between 10 and 1000 are specified, the line will wrap at the specified size when the screen size is larger than the specified value.

The position where the line is broken by specifying LineWidthLimit is the position of the specified number of characters in the average width of the half-width font of the size specified by FontSize. If $FIXED is specified in FontFace, it usually matches the number of characters. However, depending on the fraction of the font size after the decimal point, line breaks may occur before and after the intended digit position. Make sure to confirm the specified value by the actual display in advance.

<small><span style="color:red">Added since Ver.4.2.0</span></small>