---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.HttpTimeout Property
nav_order: 10
permalink: /package/standard/root/properties/httptimeout
---
# {{ page.title }}
<br>

Specifies the default timeout value for Biz / Browser communication in seconds.

 

If 0 is specified, the setting will be canceled and the standard timeout time for Windows will be used.

The default setting is 0.

The specified timeout value is not canceled even if Biz / Browser is initialized by the <a href="/package/standard/root/methods/login">Login</a> method. It is valid regardless of the connection destination until the Biz / Browser process ends.

Since it is initialized (not saved) after restarting Biz / Browser, normally set the HttpTimeout property in the first CRS to be executed after startup.

If you specify a value that exceeds the standard Windows timeout value, the standard Windows value takes precedence.

※ The standard timeout value for Windows is based on Microsoft specifications.

<br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.3.0.0</span></small>