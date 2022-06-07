---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.MinimizeBox Property
nav_order: 14
permalink: /package/standard/root/properties/minimizebox
---
# {{ page.title }}
<br>

Specifies whether to enable or disable the "Minimize" button in the root window.

 

If $ TRUE is specified, the "Minimize" button will be enabled and can be minimized by user operation.

Specifying $ FALSE disables the Minimize button.

(Minimization by pressing the shortcut key assigned to the "Minimize" button is also invalid.)

 

The initial value is $ TRUE.


If specify the MinimizeBox property to $ FALSE from the script while it is already minimized, the Minimize button will be disabled at that point, but the window will remain minimized.


Invalid if Biz / Browser is running inside Internet Explorer.


***Mobile Version***

Specifies the display status of the [X] button displayed on the task bar and menu bar when executed on Windows Mobile.

Setting $ FALSE hides the [X] button.

The initial value is $ TRUE.
 
Once set to $ FALSE, it will be valid until the end of Biz / Browser Mobile, and will not be displayed again even if the Login method is executed or $ TRUE is respecified.

<br><small><span style="color:red">Added since Ver.4.0.1, Mobile Ver.4.5.0</span></small>
<br><small><span style="color:blue">Not supported in AI</span></small>