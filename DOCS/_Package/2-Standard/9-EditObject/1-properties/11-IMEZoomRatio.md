---
layout: default

grand_parent: EditObject Class
parent: Properties
has_children: false
title: EditObject.IMEZoomRatio property
nav_order: 11
permalink: /package/standard/editobject/properties/imezoomratio
---
# {{ page.title }}


An integer value from 0 to 4 can be specified. If you specify a value larger than 1, the IME conversion character enlargement function will be enabled, and pressing the Ctrl + Insert key during IME input will enlarge the image at the magnification specified in the IMEZoomRatio property. Also, the <a href="/package/standard/form/events/keydown">KeyDown</a> event will no longer occur when pressing the Ctrl + Insert key.

By specifying the IMEZoomRatio property for input items that have many similar characters such as personal names and place names, you can enlarge the input characters and check them, which helps to prevent typos.

If a value less than or equal to 1 is specified, this function will be disabled and the KeyDown event will be fired when the Ctrl + Insert key is pressed.

<br><small><span style="color:red">Added since Ver.4.2.0</span></small>
<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>
