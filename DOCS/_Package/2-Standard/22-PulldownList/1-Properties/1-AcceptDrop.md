---
layout: default

grand_parent: PulldownList Class
parent: Properties
has_children: false
title: AcceptDrop Property
nav_order: 1
permalink: /package/standard/pulldownlist/properties/acceptdrop
---
# {{ page.title }}

<br>

Specifies the type that accepts drag and drop.

If specified, it will accept drag and drop. Specify a combination of the following constants.

|  Constant  | Value | Description                                                                                                                              |
|:----------:|:-----:|------------------------------------------------------------------------------------------------------------------------------------------|
|   $ FILE   |   1   | Receive a drop of a file from Explorer etc.                                                                                              |
|  $ STRING  |   2   | Receive text edit drops from Word etc.                                                                                                   |
|  $ OBJECT  |   4   | Receives a reference to the object set by the <a href="/package/extension4/dragsource/methods/setobject">DragSource.SetObject</a> method |
| $ COPYMODE |  256  | Drops are accepted in copy mode. The drag source must specify the copy mode.                                                             |
| $ MOVEMODE |  512  | Drops are accepted in move mode. The drag source must specify the move mode.                                                             |

<br><br>

**Drop Mode**

You can specify the type of drag and drop to be accepted by specifying the drop mode ($ COPYMODE, $ MOVEMODE), but in either mode, the copy or move operation is not actually performed.

Please decide the copy or move by the application and implement it.

<br><br>

**Caution when specify $ MOVEMODE**

If both $ COPYMODE and $ MOVEMODE are omitted, it will operate as copy mode, but if only $ MOVEMODE is specified, copy mode will be canceled.

To specify both copy mode and move mode, use $ COPYMODE + $ MOVEMODE.

<br><br>

**Drop mode change by key operation**

If $ COPYMODE is specified in AcceptDrop, drag and drop in move mode will not be accepted, but you can forcibly change to copy mode and accept drops by pressing the Ctrl key.

 

Similarly, if $ MOVEMODE is specified, drag and drop in copy mode will not be accepted, but you can forcibly change to move mode and accept drops by pressing the Shift key.

<small><span style="color:red">Added since Ver.4.1.0</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>