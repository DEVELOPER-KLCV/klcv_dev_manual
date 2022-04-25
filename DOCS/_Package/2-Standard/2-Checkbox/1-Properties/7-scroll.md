---
layout: default

grand_parent: CheckBox Class
parent: Properties
has_children: false
title: Scroll property
nav_order: 7
permalink: /package/standard/checkbox/properties/scroll
---
# {{ page.title }}

Controls the display of the scroll bar.

| Constant | Value | Description |
|----------|-------|-------------|
|$AUTO     | 0     | Automatic display<br>The scroll bar is automatically displayed or hidden according to the size of the displayed content. |
|$NONE     | 1     | None<br>Not always displayed regardless of the size of the displayed content.<br>It is not possible to scroll to the contents beyond the display range. |
|$STATIC   | 2     | Fixed display<br>Always display regardless of the size of the displayed content. |

<b>Restrictions on Mobile version</b>

The specification of $ STATIC is ignored.<br>
**<small>Restrictions are removed since Mobile Version 3.0.0</small>**
