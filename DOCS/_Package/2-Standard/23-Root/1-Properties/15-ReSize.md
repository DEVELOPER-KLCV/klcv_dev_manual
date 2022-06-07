---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.ReSize Property
nav_order: 15
permalink: /package/standard/root/properties/resize
---
# {{ page.title }}
<br>

Specifies whether to allow or prohibit resizing of the root window.

 

Setting $ TRUE allows the user to change the window size.

Setting $ FALSE prohibits the user from changing the window size. However, it can still be maximized and minimized. To prevent maximization and minimization and completely fix the window size, use the MinimizeBox and MaxmizeBox properties.

 
Invalid if Biz / Browser is running inside Internet Explorer.


<br><small><span style="color:green">The following parameters can be specified since Ver.5.0.0</span></small><br>
If $ SYNC is set, resizing will be performed while maintaining the aspect ratio.

<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>
