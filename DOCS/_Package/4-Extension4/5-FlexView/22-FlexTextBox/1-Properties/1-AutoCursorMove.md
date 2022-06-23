---
layout: default

grand_parent: FlexTextBox Class
parent: Properties
has_children: false
title: FlexTextBox.AutoCursorMove Property
nav_order: 1
permalink: /package/extension4/flexview/flextextbox/properties/autocursormove
---
# {{ page.title }}

Set to true to automatically move the cell cursor.

If set to true, the cell cursor will move in the same way as when the right arrow key is pressed at the next opportunity.

-When the input content is confirmed by pressing the Enter key.<br>
-When the key input of the number of characters specified in the MaxLength property is performed.

If the cursor does not move when you press the right arrow key, such as at the end of a line, the cell cursor does not move even if you specify the AutoCursorMove property to true, but the input content is confirmed and the TextChanged event occurs if there is a change. 

<small><span style="color:red">Added since Ver.4.1.0</span></small>