---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.UseChange Property
nav_order: 219
permalink: /package/extension5/sspread/properties/usechange
---
# {{ page.title }}
 
Specifying a value is invalid for this class.

The <a href="/package/system/netobject/properties/usechange">UseChange</a> property of the inherited class sets whether to raise the <a href="/package/system/netobject/events/change">Change</a> event by changing the default property (mainly the Value property), but this class behaves differently from other classes in the following points.

· This class has no default properties<br>
· <a href="/package/extension5/sspread/properties/value">SSpread.Value</a> property is not the default property<br>
· <a href="/package/extension5/sspread/events/change">SSpread.Change</a> event does not occur when the default property changes

From the above, specifying a value for this property has no effect.
