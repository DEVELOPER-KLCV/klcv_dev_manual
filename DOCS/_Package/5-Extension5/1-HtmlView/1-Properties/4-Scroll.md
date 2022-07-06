---
layout: default

grand_parent: HtmlView Class
parent: Properties
has_children: false
title: Scroll Property
nav_order: 4
permalink: /package/extension5/htmlview/properties/scroll
---
# {{ page.title }}

Controls the display of the scroll bar.

| Constant | Value | Description                                                                                                                                       |
|----------|:-----:|---------------------------------------------------------------------------------------------------------------------------------------------------|
| $AUTO    |   0   | Automatic display <br> The scroll bar is automatically displayed or hidden according to the size of the displayed content.                             |
| $NONE    |   1   | None <br>Not always displayed regardless of the size of the displayed content. <br>It is not possible to scroll to the contents beyond the display range. |
| $STATIC  |   2   | Fixed display <br>Always display regardless of the size of the displayed content.                                                                     |

***Restrictions on Mobile version***<br>
The specification of $STATIC is ignored.<br><small><span style="color:green">No more restriction since Mobile Ver.3.0.0</span></small>
