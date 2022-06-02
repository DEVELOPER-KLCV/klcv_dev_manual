---
layout: default

grand_parent: OptionItem Class
parent: Events
has_children: false
title: OptionItem.Touch Property
nav_order: 1
permalink: /package/standard/optionitem/events/touch
---
# {{ page.title }}
<br>

This event occurs when you change the options of the option button.

It occurs regardless of the operation from the screen or the operation from the script.

 

 

***Note***
In the handler of the event that occurred in the OptionItem class, do not use the <a href="/package/standard/optionbutton/properties/value">Value</a>
 property of the parent object <a href="/package/standard/optionbutton">OptionButton</a> class to refer to the selected item number. (The selected item number may not be reflected.)

For the selected item number, refer to the Index property (subscript of the array) of the <a href="/package/system/event/properties/from">From</a> property (OptionItem object) of the <a href="/package/system/event">Event</a> object passed as an argument of the event handler.