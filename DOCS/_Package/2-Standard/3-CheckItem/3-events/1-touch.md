---
layout: default

grand_parent: CheckItem Class
parent: Properties
has_children: false
title: CheckItem.Touch Event
nav_order: 1
permalink: /package/standard/checkitem/events/touch
---
# {{ page.title }}

This event occurs when the selected state of the check box is changed.
It occurs regardless of the operation from the screen or the operation from the script.
 
<b>Note</b>
In the handler of the event generated in CheckItem class, do not use the [Value](/package/standard/checkbox/properties/value) property of [CheckBox](/package/standard/checkbox) class which is the parent object to refer to the selected item number. (The selected item number may not be reflected.)

For the selected item number, refer to the Index property (array subscript) of the [From](/package/system/event/properties/from) property (CheckItem object) of the [Event](/package/system/event) object passed as an argument of the event handler. For the selected state of the item, refer to the [Selected](/package/standard/checkitem/properties/selected) property from the From property.
