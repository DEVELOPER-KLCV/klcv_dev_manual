---
layout: default

grand_parent: FlexItem Class
parent: Properties
has_children: false
title: FlexItem.TitleResize Property
nav_order: 6
permalink: /package/extension4/flexview/flexitem/properties/titleresize
---
# {{ page.title }}

Specify whether to resize the column width by mouse operation of the column title.

If true is specified, the column width can be changed by dragging the column border with the mouse.
If false is specified, the column width will be fixed.

Changing the column width is limited to columns that consist of a single FlexItem. Boundaries involving multiple columns in combination with FlexColumnSet and FlexRowSet cannot be changed regardless of the TitleResize property specified.

<small><span style="color:red">Added since Ver.4.1.0</span></small>
<br><small><span style="color:blue">Not supported in AI</span></small>