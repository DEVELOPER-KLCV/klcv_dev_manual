---
layout: default

grand_parent: MaskEdit Class
parent: Properties
has_children: false
title: MaskEdit.InputMode Property
nav_order: 5
permalink: /package/extension4/maskedit/properties/inputmode
---
# {{ page.title }}

Specify the character types that can be entered.
See <a href="/package/extension4/maskedit/properties/inputmode">InputMode</a> for possible values.

Specifying the InputMode property has nothing to do with specifying the <a href="/package/extension4/maskedit/properties/mask">Mask</a> property.
Only characters that meet both the Mask and InputMode properties can be entered.

For example, if you specify "CC" indicating a character input field in the Mask property and $ZENKAKU in the InputMode property, only full-width characters can be input only in the specified position.