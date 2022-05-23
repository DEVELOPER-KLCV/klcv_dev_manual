---
layout: default

grand_parent: Form Class
parent: Properties
has_children: false
title: Scroll property
nav_order: 9
permalink: /package/standard/form/properties/scroll
---
# {{ page.title }}



<br>

Controls the display of the scroll bar.

| Constant   | Value | Description                                                                                                                                       |
|------------|:-----:|---------------------------------------------------------------------------------------------------------------------------------------------------|
| $ AUTO     |   0   | Automatic display The scroll bar is automatically displayed or hidden according to the size of the displayed content.                             |
| $ NONE     |   1   | none Not always displayed regardless of the size of the displayed content. It is not possible to scroll to the contents beyond the display range. |
| $ STATIC   |   2   | Fixed display Always display regardless of the size of the displayed content.                                                                     |
| $ COPYMODE |  256  | Drops are accepted in copy mode. The drag source must specify the copy mode.                                                                      |
| $ MOVEMODE |  512  | Drops are accepted in move mode. The drag source must specify the move mode.                                                                      |

<br>
**Restrictions on Mobile version**

Ignore the specification of $ STATIC.
<br><small><span style="color:green">No more restrictions since Mobile Ver.3.0.0</span></small>