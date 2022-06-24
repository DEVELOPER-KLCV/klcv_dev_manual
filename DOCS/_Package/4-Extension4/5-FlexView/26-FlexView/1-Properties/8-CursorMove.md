---
layout: default

grand_parent: FlexView Class
parent: Properties
has_children: false
title: FlexView.CursorMove Property
nav_order: 8
permalink: /package/extension4/flexview/flexview/properties/cursormove
---
# {{ page.title }}
<br>

Specifies how to move the cell cursor with the left and right arrow keys.

**$STD** <br>
Moves to individual cells except the header system.

**$INPUTITEM**<br>
Selectively move to a cell that can be operated by the user. Manipulable cells are cells generated from FlexButton, FlexTextBox, etc.

**$ENTER**<br>
The Enter key moves the cell cursor in the same way as the right arrow key. You can also use the Shift + Enter keys to move the cell cursor in the same way as the left arrow key.

**$LINEFEED**<br>
It automatically moves from the end of the line to the beginning of the next line, or from the beginning of the line to the end of the previous line.

If the next line is the FlexTreeHeader header line, the header line will be skipped. <br><small><span style="color:green">Extension since Ver.5.0.2</span></small>

**$LINEUP**
<br><small><span style="color:red">Added since Ver.4.1.4</span></small> <small><span style="color:blue">Not supported in Mobile, AI</span></small><br>

The cell cursor automatically moves to the right The next operation moves the cell cursor in the same way as the down arrow key. $ LINEUP cannot be specified at the same time as $ INPUTITEM and $ LINEFEED.<br>

| FlexTextBox | Confirmation operation by ENTER key of AutoCursorMove = $TRUE <br>Input confirmation operation by AutoCursorMove = $TRUE and MaxLength |
| FlexView    | Pressing the ENTER key with CursorMove = $ENTER + $LINEUP                                                                          |

**$SKIPHIDDENCOL**<br>
<small><span style="color:red">Added since Ver.5.0.2</span></small> <small><span style="color:blue">Not supported in Mobile, AI</span></small><br>
Columns with a Width of 0 are skipped.

If you want to specify multiple actions above at the same time, add them together. For example, if you specify $INPUTITEM + $LINEFEED, both $INPUTITEM operation and $LINEFEED operation will be performed. Also, if you specify $INPUTITEM + $ENTER, both $INPUTITEM operation and $ENTER operation are performed.
<br><small><span style="color:red">Added since Ver.4.1.0</span></small>
