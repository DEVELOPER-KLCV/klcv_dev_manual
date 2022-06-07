---
layout: default

grand_parent: Root Class
parent: Properties
has_children: false
title: Root.AltKeyPriority Property
nav_order: 1
permalink: /package/standard/root/properties/altkeypriority
---
# {{ page.title }}
<br>

Change the <a href="/package/standard/focusobject/properties/nexttabkey">NextTabKey</a> property, <a href="/package/standard/button/properties/altkey">AltKey</a> property, the unique behavior of the target object, and the priority of raising the <a href="/package/standard/form/events/keydown">KeyDown</a> event.

It also controls whether the KeyDown event occurs.

| Constant | Description                                     |
|:--------:|-------------------------------------------------|
|     0    | NextTabKey → Object behavior → AltKey → KeyDown |
|     1    | AltKey → NextTabKey → Object behavior → KeyDown |
|     2    | NextTabKey → AltKey → Object behavior → KeyDown |

In addition, when there is an input corresponding to NextTabKey and AltKey, the KeyDown event does not occur because each process has priority, but if "16" is added to the above setting value, the operation of specifying the NextTabKey property before the object operation , The KeyDown event is also generated at the same time as the operation of specifying the AltKey property is performed.

The operation priority when the above is taken into consideration is as follows.

| Constant | Description                                                          |
|:--------:|----------------------------------------------------------------------|
|    16    | NextTabKey + KeyDown → Object operation → AltKey → KeyDown           |
|    17    | AltKey + KeyDown → NextTabKey + KeyDown → Object operation → KeyDown |
|    18    | NextTabKey + KeyDown → AltKey + KeyDown → Object operation → KeyDown |

The initial value is 0 .

<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>

