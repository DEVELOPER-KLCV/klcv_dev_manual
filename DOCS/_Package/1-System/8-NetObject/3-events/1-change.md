---
layout: default

grand_parent: NetObject Class
parent: Events
has_children: false
title: NetObject.Change Event
nav_order: 1
permalink: /package/system/netobject/events/change
---
# {{ page.title }}


An event that occurs when the default property of an object with the <a href="/package/system/netobject/properties/usechange">UseChange property set to $ TRUE changes.<br><br>

 

Since the Change event occurs when the default property changes, it can be used when the behavior is linked to the change of the object value.<br><br>

 

In many classes, changes in the default properties trigger another class-specific event. For example, in the TextBox class, the Touch event is fired when there is input . If there is input, it will be stored in the value of the default property, so setting the UseChange property to $ TRUE will also generate a Change event at the same time, but it is usually more efficient to use the Touch event.<br><br>

 

It makes sense to use the Change event with the UseChange property set to $ TRUE for classes where the event does not occur for operations that change the default property. For example, in the String class, the event does not occur even if the Value property changes. If you need to monitor a String object and react to changes in its value, setting the UseChange property to $ TRUE raises the Change event.<br><br>
 

Another use is when you want to handle the change of value by screen input and script with a common event handler. For example, if you set the UseChange property to $ TRUE in the TextBox class, keystrokes from the screen will fire the Touch and Change events, and changing values ​​from the script will only fire the Change event.

 