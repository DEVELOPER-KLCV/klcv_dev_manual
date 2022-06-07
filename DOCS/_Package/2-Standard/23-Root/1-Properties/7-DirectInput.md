---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.DirectInput Property
nav_order: 7
permalink: /package/standard/root/properties/directinput
---
# {{ page.title }}
<br>

Specifies how to handle keystroke events internally for Biz / Browser.

Normally, the key input event for Biz / Browser reaches Biz / Browser via IME etc. after being supplemented by the OS and is delivered to each screen object, but by using this property, some of the flow of key input event processing can be changed.

If you specify $ TRUE, Biz / Browser bypasses the OS standard keystroke event and issues the keystroke event directly to the object with focus.

If $ FALSE is specified, OS standard key input event processing will be performed.

The initial value is $ FALSE.

<br><span style="color:red"><b>Notes on use</b></span>

This property forces a change in normal Biz / Browser keystroke event handling.

Therefore, the IME status may not be taken into consideration and the input may be half-width, or the shortcut keys on some screen display objects may not work.

It is recommended to use it only when a problem such as input from a bar code reader is not performed correctly when a large amount of input is performed momentarily.


<br><small><span style="color:red">Added since Ver.5.0.3</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>