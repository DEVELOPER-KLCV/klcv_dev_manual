---
layout: default

grand_parent: NumberEdit Class
parent: Events
has_children: false
title: NumberEdit.Touch Event
nav_order: 2
permalink: /package/extension3/numberedit/events/touch
---
# {{ page.title }}
<br>

This event occurs when the value changes due to an input operation from the screen.

The Touch event occurs when a value change is confirmed by pressing the Enter key or function key, or when it loses focus and is confirmed. It does not occur for each key input character.

When a format (N) that does not display empty data is specified in the <a href="/package/extension3/numberedit/properties/format">Format</a> property, the value does not change when 0 is entered from the blank, or when 0 is displayed and the Delete key is used to make it blank, but the Touch event It will be a condition of occurrence.