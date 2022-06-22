---
layout: default

grand_parent: FlexListBox Class
parent: Properties
has_children: false
title: FlexListBox.AutoCursorMove Property
nav_order: 2
permalink: /package/extension4/flexview/flexlistbox/properties/autocursormove
---
# {{ page.title }}

Set to true if you want the cell cursor to move automatically.

If set to true, the cell cursor will move in the same way as when the right arrow key is pressed at the next opportunity.

-When the input content is confirmed by pressing the Enter key.

If the cursor does not move when the right arrow key is pressed, such as at the end of a line, the cell cursor does not move even if the AutoCursorMove property is set to true, but the input content is confirmed and the SelectChanged event occurs if there is a change.
<br><small><span style="color:red">Added since Ver.4.1.0</span></small>