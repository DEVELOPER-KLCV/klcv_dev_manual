---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.InputTimeout Property
nav_order: 12
permalink: /package/standard/root/properties/inputtimeout
---
# {{ page.title }}
<br>

Specifies the timeout period for input operations.

The initial value is 120 milliseconds. This property does not need to be changed in most cases.

Biz / Browser does not handle keystrokes and mouse click input operations at the same time as script execution. If the script was executed at the time of the input operation, wait for the script to finish for a certain period of time, and if the script still does not finish, discard the input operation.

The InputTimeout property can change this wait time.

Set the InputTimeout property to a longer value if you do not want to discard the input because the input may be held for a certain period of time, such as performing heavy processing in the event handler that operates by key input or mouse click.

Conversely, if you do not want subsequent keystrokes or mouse clicks to fire as much as possible, set the InputTimeout property to a shorter value.

The InputTimeout property is a fine-tuning feature that balances input operations and script execution. Setting the InputTimeout property does not guarantee that the discarding of input events will be completely suppressed or that consecutive events will be completely discarded.

Many aspects that require the InputTimeout property to be set contradict the basic CRS rule that the order in which events occur is not guaranteed. Consider reviewing the processing method before setting the InputTimeout property.

The InputTimeout property can be specified in the range of 80 milliseconds to 1000 milliseconds.

The settings are reset to 120 milliseconds when Biz / Browser is initialized by calling the <a href="/package/standard/root/methods/login">Login</a> method.

<br><small><span style="color:red">Added since Ver.4.1.4</span></small>
<br><small><span style="color:blue">Not supported in Mobile</span></small>