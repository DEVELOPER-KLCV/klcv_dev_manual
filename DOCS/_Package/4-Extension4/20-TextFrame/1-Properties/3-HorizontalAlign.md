---
layout: default

grand_parent: TextFrame Class
parent: Properties
has_children: false
title: TextFrame.HorizontalAlign Property
nav_order: 3
permalink: /package/extension4/textframe/properties/horizontalalign
---
# {{ page.title }}

Performs horizontal alignment. $STD is right-aligned if the data type is Number, Fixed type, and left-aligned otherwise.

| Constant | Value | Description   |
|----------|:-----:|---------------|
| $STD    |   0   | Determined by data type |
| $LEFT   |   1   | Left-aligned    |
| $CENTER |   2   | Centered      |
| $RIGHT  |   3   | Right-aligned   |

If specify $CENTER or $RIGHT, the horizontal scroll bar is not displayed regardless of the <a href="/package/extension4/textframe/properties/scrollbarposition">ScrollBarPosition</a> property.