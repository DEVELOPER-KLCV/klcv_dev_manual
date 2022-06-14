---
layout: default

grand_parent: TextBox Class
parent: Properties
has_children: false
title: TextBox.AutoComplete Property
nav_order: 1
permalink: /package/standard/textbox/properties/autocomplete
---
# {{ page.title }}
<br>

Specify ON / OFF of text completion. The initial value is $ FALSE.

Character strings entered with text completion are not subject to input restrictions due to the setting of the <a href="/base/inputmode">InputMode</a> property. Specifying the <a href="/package/standard/editbox/properties/maxlength">MaxLength</a> property is valid, but the <a href="/package/standard/editbox/properties/maxlengthreached">MaxLengthReached</a> event does not occur.

Also, the setting of the <a href="/package/standard/editbox/properties/autotab">AutoTab</a>  property is ignored.

<br><br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>