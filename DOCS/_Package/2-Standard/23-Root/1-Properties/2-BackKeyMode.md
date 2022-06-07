---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.BackKeyMode Property
nav_order: 2
permalink: /package/standard/root/properties/backkeymode
---
# {{ page.title }}

Specifies the behavior when the "Back" button is clicked.

 

Specify a combination of the following constants, or specify 0.

|        Constant       |                                 Description                                |
|:---------------------:|:--------------------------------------------------------------------------:|
| Root.ConfirmClose = 1 | A completion confirmation message is displayed when the button is pressed. |
| Root.RaiseKeyDown = 2 | A KeyDown event is issued when the button is pressed .                     |

If 0 is specified, the end confirmation message will not be displayed and the KeyDown event will not be issued.

When Root.ConfirmClose is specified, the end confirmation message is displayed by pressing the button for the first time, and the Close event is issued by pressing the button a second time.

If not specified, the Close event is issued immediately.

 

The initial value is Root.ConfirmClose + Root.RaiseKeyDown.

<br><small><span style="color:red">Added since AI Ver.1.0.2</span></small>

