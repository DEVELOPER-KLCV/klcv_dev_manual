---
layout: default

grand_parent: ContainerObject Class
parent: Properties
has_children: false
title: ContainerObject.PrevTabKey property
nav_order: 2
permalink: /package/standard/containerobject/properties/prevtabkey
---
# {{ page.title }}

If the object managed as a child has keyboard focus , pressing the key specified in the PrevTabKey property moves the keyboard focus to the previous object.<br><br>

 

If the child object has its own focus move key, the child object's specification takes precedence.<br><br>

Also, if the key specified in the PrevTabKey property is used as a unique function of the child object, the processing of the child object is prioritized and the focus is not moved.<br><br>

 

For the values ​​that can be specified for the PrevTabKey property, refer to [Key specification](/base/key).<br><br>

 

For the priority when multiple meanings are assigned to one key operation, refer to [Priority in key operation](/base/key#priority-order-for-key-operations).

<small>There are restrictions on the keys that can be specified in AI. See [Android version features and constraints](/bizBrowserV/2/2-5/)</small>
