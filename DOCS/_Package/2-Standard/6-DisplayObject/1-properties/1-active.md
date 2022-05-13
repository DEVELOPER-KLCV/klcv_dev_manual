---
layout: default

grand_parent: DisplayObject Class
parent: Properties
has_children: false
title: DisplayObject.Active property
nav_order: 1
permalink: /package/standard/displayobject/properties/active
---
# {{ page.title }}


Setting $ TRUE activates the object and reacts to user interaction.

Setting $ FALSE deactivates the object and stops accepting user actions.

 

Objects located below the object for which $ FALSE is set will not accept operations at the same time, but the display status will not change.

 

If you change it to $ FALSE while it is in focus, the focus will move to the first object in that window that can receive focus.

 

