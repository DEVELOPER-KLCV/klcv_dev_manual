---
layout: default

grand_parent: ListItem Class
parent: Events
has_children: false
title: ListItem.Touch Property
nav_order: 1
permalink: /package/standard/listitem/events/touch
---
# {{ page.title }}
<br>

An event that occurs when an item in the list box is selected.
It occurs regardless of the operation from the screen or the operation from the script.

Occurs when the <a href="/package/standard/listbox/properties/selectionmode">SelectionMode</a> property of the <a href="/package/standard/listbox">ListBox</a> class changes from OFF to ON if it is $ STD.

If the SelectionMode property of the ListBox class is $ MULTI, it will occur for both OFF to ON and ON to OFF changes.

***Note*** <br>
In the handler of the event that occurred in the ListItem class, do not use the <a href="/package/standard/listbox/properties/value">Value</a> property of the parent object <a href="/package/standard/listbox">ListBox</a> class to refer to the selected item number. (The selected item number may not be reflected.)

For the selected item number, refer to the Index property (subscript of the array) of the <a href="/package/system/event/properties/from">From</a> property (ListItem object) of the <a href="/package/system/event">Event</a> object passed as an argument of the event handler. For the selected state of the item, refer to the <a href="/package/standard/listitem/properties/selected">Selected</a> property from the From property. 