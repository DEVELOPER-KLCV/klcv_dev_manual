---
layout: default

grand_parent: FocusObject Class
parent: Events
has_children: false
title: FocusObject.FocusOperation Event
nav_order: 1
permalink: /package/standard/focusobject/events/focusoperation
---
# {{ page.title }} 


This event occurs when you perform a key input operation that causes the focus to move while the object is receiving keyboard focus. The <a href="/package/standard/focusoperationevent">FocusOperationEvent</a> object is passed to the event handler .
 

The operation that causes the focus to move is the operation that the Tab key or <a href="/package/standard/focusobject/properties/nexttabkey">NextTabKey</a>, the key set in the <a href="/package/standard/focusobject/properties/prevtabkey">PrevTabKey</a> property is pressed, and the focus is moved by the AutoTab property for the class that has the AutoTab property.

The FocusOperation event does not occur for operations other than these .

 

The FocusOperation event occurs exclusively with focus movement, as specified by the <a href="/package/standard/focusobject/properties/autotabfocus">AutoTabFocus</a> property, which directs automatic focus movement .

If the AutoTabFocus property is $ TRUE , the operation that causes the focus move will move the focus and the FocusOperation event will not be fired.

If the AutoTabFocus property is $ FALSE , the focus will not move and the FocusOperation event will be fired.

<br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.2.0.</span></small>