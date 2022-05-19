---
layout: default

grand_parent: EditBox Class
parent: Properties
has_children: false
title: EditBox.HorizontalAlign property
nav_order: 2
permalink: /package/standard/editbox/properties/horizontalalign
---
# {{ page.title }}

Performs horizontal alignment. $ STD is right-aligned if the data type is Number, Fixed type, and left-aligned otherwise.

| Constant | Value | Description             |
|----------|:-----:|-------------------------|
| $ STD    |   0   | Determined by data type |
| $ LEFT   |   1   | Left-aligned            |
| $ CENTER |   2   | Centered                |
| $ RIGHT  |   3   | Right-aligned           |



If you specify $ CENTER or $ RIGHT, the horizontal scrollbar is not displayed regardless of the <a href="/package/standard/editbox/properties/scrollbarposition">ScrollBarPosition</a> property.