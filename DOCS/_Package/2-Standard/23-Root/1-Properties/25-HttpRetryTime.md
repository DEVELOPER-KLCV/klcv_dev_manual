---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.HttpRetryTime Property
nav_order: 25
permalink: /package/standard/root/properties/httpretrytime
---
# {{ page.title }}
<br>

This property is only valid when using a dial-up connection.

When connecting / disconnecting a dial-up connection repeatedly, the response may not be established without establishing an HTTP connection because the previous connection information remains at the time of the first communication after the dial-up connection.

In that case, specify the timeout period until the HTTP connection is forcibly disconnected and reconnected. 0 is not specified and depends on the timeout time of the OS.

The HttpRetryTime property can be specified in the range of 0, 1 to 28800 seconds. The setting value is not reset even if Biz / Browser is initialized by the <a href="/package/standard/root/methods/login">Login</a> method.

<br><small><span style="color:red">Can only be used with Mobile</span></small>
<br><small><span style="color:red">Added since Mobile Ver.4.0.0</span></small>