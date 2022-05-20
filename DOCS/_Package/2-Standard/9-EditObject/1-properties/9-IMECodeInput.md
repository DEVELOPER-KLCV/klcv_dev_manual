---
layout: default

grand_parent: EditObject Class
parent: Properties
has_children: false
title: EditObject.IMECodeInput property
nav_order: 9
permalink: /package/standard/editobject/properties/imecodeinput
---
# {{ page.title }}


If $ TRUE is specified, the character code will be entered in 4-digit hexadecimal number during IME conversion, and it will be converted to the corresponding character by pressing the Ctrl + Home key. Unlike the input from the character code list using the F5 key provided by IME as standard, it is directly converted to characters without popping up the IME pad. Also, the <a href="/package/standard/form/events/keydown">KeyDown</a> event will no longer occur when pressing the Ctrl + Home key.

Specifying $ FALSE disables this feature, and pressing Ctrl + Home raises the KeyDown event.


<br><small><span style="color:red">Added since Ver.4.2.0</span></small>
<br><small><span style="color:grey">It is always invalid when running on Windows Vista or later OS, since Ver5.0.2</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>