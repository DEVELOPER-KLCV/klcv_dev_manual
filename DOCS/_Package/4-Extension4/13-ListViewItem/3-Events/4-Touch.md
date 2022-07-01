---
layout: default

grand_parent: ListViewItem Class
parent: Events
has_children: false
title: ListViewItem.Touch Event
nav_order: 4
permalink: /package/extension4/listviewitem/events/touch
---
# {{ page.title }}

This event occurs when ListViewItem is selected.


It occurs regardless of the operation from the screen or the operation from the script.

Occurs when the ListView's SingleSel property is $TRUE and changes from OFF to ON.

When the SingleSel property of ListView is $FALSE, it occurs in both OFF to ON and ON to OFF changes.

The Touch event also occurs when changing from the selected state to the unselected state or when pressing PageDown / PageUp with SingleSel = $FALSE.

If you reselect the same location, the Touch event will not fire if SingleSel = $TRUE, and the Touch event will fire if $FALSE. (OFF → ON occurs)

<a href="/package/extension4/listviewitem/events/#precautions-when-referring-to-selection-items">Precautions when referring to selection items</a>