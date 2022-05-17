---
layout: default

grand_parent: DisplayObject Class
parent: Events
has_children: false
title: DisplayObject.Timer Event
nav_order: 6
permalink: /package/standard/displayobject/events/timer
---
# {{ page.title }}


Occurs when the time set by the <a href="/package/standard/displayobject/methods/settimer">SetTimer</a> method has elapsed.

 

Be careful when performing time-consuming processing in the event handler of the Timer event. Since Timer events occur repeatedly at specified intervals, if processing that takes longer than the Timer event occurrence interval is performed, Timer events may accumulate in the event queue and become inoperable.

 

To stop the Timer event, call the <a href="/package/standard/displayobject/methods/removetimer">RemoveTimer</a> method.

