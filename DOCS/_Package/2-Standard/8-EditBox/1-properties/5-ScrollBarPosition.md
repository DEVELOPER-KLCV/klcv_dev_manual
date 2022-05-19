---
layout: default

grand_parent: EditBox Class
parent: Properties
has_children: false
title: EditBox.ScrollBarPosition property
nav_order: 5
permalink: /package/standard/editbox/properties/scrollbarposition
---
# {{ page.title }}

Set the display position of the scroll bar.

| Constant  | Value | Description                                 |
|-----------|:-----:|---------------------------------------------|
| $ STD     |   0   | Display vertical and horizontal scroll bars |
| $ VSCROLL |   2   | Show vertical scrollbar                     |
| $ HSCROLL |   3   | Show horizontal scroll bar                  |
| $ NONE    |   1   | Hide scrollbars                             |

If $ NONE is specified, the input from the screen will be up to the number of displayed characters.

If the <a href="/package/standard/editbox/properties/verticalalign">HorizontalAlign</a> property is $ CENTER or $ RIGHT, the horizontal scroll bar will not be displayed regardless of the specification of this property.


**Restrictions on Mobile version**<br>
Due to OS restrictions , $ HSCROLL is disabled for HorizontalAlign = $ CENTER , $ RIGHT or Number types.

