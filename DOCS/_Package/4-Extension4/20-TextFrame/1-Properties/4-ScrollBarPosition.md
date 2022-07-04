---
layout: default

grand_parent: TextFrame Class
parent: Properties
has_children: false
title: TextFrame.ScrollBarPosition Property
nav_order: 4
permalink: /package/extension4/textframe/properties/scrollbarposition
---
# {{ page.title }}


Set the display position of the scroll bar.

| Constant  | Value | Description                                |
|-----------|:-----:|--------------------------------------------|
| $ STD     |   0   | Display vertical and horizontal scroll bar |
| $ NONE    |   1   | Don't show scroll bar                      |
| $ VSCROLL |   2   | Show vertical scroll bar                   |
| $ HSCROLL |   3   | Show horizontal scroll bar                 |

If the <a href="/package/extension4/textframe/properties/horizontalalign">HorizontalAlign</a> property is $CENTER or $RIGHT, the horizontal scroll bar will not be displayed regardless of the specification of this property.