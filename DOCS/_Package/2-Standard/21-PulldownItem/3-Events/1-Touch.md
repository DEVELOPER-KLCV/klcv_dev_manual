---
layout: default

grand_parent: PulldownItem Class
parent: Events
has_children: false
title: PulldownItem.Touch Property
nav_order: 1
permalink: /package/standard/pulldownitem/events/touch
---
# {{ page.title }}
<br>

An event that occurs when an item in the pull-down list is selected.

It occurs regardless of the operation from the screen or the operation from the script.


***Note***<br>

In the handler of the event that occurred in the PulldownItem class, do not use the <a href="/package/standard/pulldownitem/properties/value">Value</a> property of the parent object <a href="/package/standard/pulldownlist">PulldownList</a> class to refer to the selected item number. (The selected item number may not be reflected.)

For the selected item number, refer to the Index property (subscript of the array) of the <a href="/package/system/event/properties/from">From</a> property (PulldownItem object) of the <a href="/package/system/event">Event</a> object passed as an argument of the event handler.
