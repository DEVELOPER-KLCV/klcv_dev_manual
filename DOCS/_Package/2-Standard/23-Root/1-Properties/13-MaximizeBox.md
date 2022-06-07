---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.MaximizeBox Property
nav_order: 13
permalink: /package/standard/root/properties/maximizebox
---
# {{ page.title }}
<br>

Specifies whether to enable or disable the "Maximize" button in the root window.

 

If $ TRUE is specified, the "Maximize" button will be enabled and can be maximized by user operation.

Specifying $ FALSE disables the Maximize button.

(Maximization by pressing the shortcut key assigned to the "Maximize" button is also invalid.)


The initial value is $ TRUE.

 

If specify the MaximizeBox property to $ FALSE while it is already maximized, the Maximize button will be disabled, but the display size of the window will remain the same.


Invalid if Biz / Browser is running inside Internet Explorer.

<br><small><span style="color:red">Added since Ver.4.0.1</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>