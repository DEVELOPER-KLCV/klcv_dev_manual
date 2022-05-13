---
layout: default

grand_parent: DisplayObject Class
parent: Properties
has_children: false
title: DisplayObject.TabIndex property
nav_order: 4
permalink: /package/standard/displayobject/properties/tabindex
---
# {{ page.title }}


Shows the display and input priority of objects.

 

The smaller the value, the earlier the keyboard focus will be received. Also, the smaller the value, the closer it is displayed, that is, it is placed in the foreground in the depth direction.

 

The order in which the keyboard focus is moved by the TabIndex property works only between objects in the same hierarchy. You cannot specify the order of keyboard focus between objects in different hierarchies.

 

For arrayed objects, you cannot specify the TabIndex property for individual objects that are array elements . Focus movements within an array are always from front to back of the array elements.

 

***Note*** 
<br>The TabIndex specification is invalid for DisplayObjects that are dynamically generated (Get method, Append method, etc.) other than when Form is initialized, and the movement order by tabs is set to the lowest level among DisplayObjects in the same hierarchy .

