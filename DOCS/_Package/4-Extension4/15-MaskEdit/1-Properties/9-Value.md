---
layout: default

grand_parent: MaskEdit Class
parent: Properties
has_children: false
title: MaskEdit.Value Property
nav_order: 9
permalink: /package/extension4/maskedit/properties/value
---
# {{ page.title }}

The value to be displayed in the mask edit.

If the entered value does not meet the specified conditions of the <a href="/package/extension4/maskedit/properties/mask">Mask</a>  property, it will be an empty character string.

It does not include edit literal characters added by the Mask property.

Contains characters entered in the input field and blank characters that appear in unfilled positions (default is underscore "_").

A string containing edit literal characters can be obtained with the <a href="/package/extension4/maskedit/properties/edittext">EditText</a>  property.

Scripted value settings are not validated by the Mask property and are not affected by the <a href="/package/extension4/maskedit/properties/inputmode">InputMode</a>  property.

Specify a character string that is consistent with the contents specified in the Mask property.

The input value on the screen is not reflected immediately. Refer to the <a href="/package/standard/editobject/#timing-the-value-property-updated">Timing the Value Property Updated</a> for more information.