---
layout: default

grand_parent: FocusObject Class
parent: Properties
has_children: false
title: FocusObject.AutoTabFocus property
nav_order: 1
permalink: /package/standard/focusobject/properties/autotabfocus
---
# {{ page.title }}


Setting $ TRUE moves the focus to the next tabbed object during the following operations:

-Pressing the Tab key or the key set in the <a href="/package/standard/focusobject/properties/nexttabkey">NextTabKey</a> or <a href="/package/standard/focusobject/properties/prevtabkey">PrevTabKey</a> property

-For classes with the AutoTab property, the operation performed by the AutoTab property is executed.

If you set $ FALSE, the focus will no longer move automatically, only with the <a href="/package/standard/focusobject/methods/setfocus">SetFocus</a> and <a href="/package/standard/focusobject/methods/movefocus">MoveFocus</a> methods from the user's mouse operation or script. 

However, the LostFocus event is fired by switching windows (including pop-ups from Biz / Browser itself, such as dialogs and message boxes). Also, if the focus cannot be maintained, such as by deleting the object that is in focus, the focus will move to another object.

If you press the Tab key or NextTabKey, the key set in the PrevTabKey property, or operate the AutoTab property with $ FALSE set, the <a href="/package/standard/focusobject/events/focusoperation">FocusOperation</a> event will be generated.

 

The initial value is $ TRUE.

<br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.2.0.</span></small>