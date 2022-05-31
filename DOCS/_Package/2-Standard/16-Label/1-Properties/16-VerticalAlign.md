---
layout: default

grand_parent: Label Class
parent: Properties
has_children: false
title: Label.VerticalAlign Property
nav_order: 16
permalink: /package/standard/label/properties/verticalalign
---
# {{ page.title }}

<br>

Performs vertical alignment. $ STD will be top-justified.

| Constant | Value |    Description   |
|:--------:|:-----:|:----------------:|
|   $ STD  |   0   |   Same as $ TOP  |
|   $ TOP  |   1   |   Top alignment  |
| $ CENTER |   2   |     Centered     |
| $ BOTTOM |   3   | Bottom alignment |


When the VerticalAlign property is specified, the characters in the Label cannot be wrapped except when printing. If you do not specify the VerticalAlign property, the characters in the Label will wrap.

<br><small><span style="color:green">It is now valid on the screen since Mobile Ver.2.0.0</span></small>