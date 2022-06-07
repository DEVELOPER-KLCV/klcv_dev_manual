---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.UseHttpPreconfig Property
nav_order: 27
permalink: /package/standard/root/properties/usehttppreconfig
---
# {{ page.title }}
<br>

Specifies whether to use standard proxy settings when communicating.

For $ TRUE, connect using standard proxy settings.

For $ FALSE, connect directly without using standard proxy settings.

The setting value is not reset even if Biz / Browser is initialized by the <a href="/package/standard/root/methods/login">Login</a> method.

The initial value is $ TRUE.

However, the initial value is $ FALSE when started by specifying "/ proxy *" in the command line option.

<br><small><span style="color:red">Can only be used with Mobile</span></small>
<br><small><span style="color:red">Added since Mobile Ver.3.1.0</span></small>