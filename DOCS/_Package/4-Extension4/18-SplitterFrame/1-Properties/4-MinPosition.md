---
layout: default

grand_parent: SplitterFrame Class
parent: Properties
has_children: false
title: SplitterFrame.MinPosition Property
nav_order: 4
permalink: /package/extension4/splitterframe/properties/minposition
---
# {{ page.title }}

Specifies the minimum value of the controllable range of the split line by mouse operation.
Combined with the <a href="/package/extension4/splitterframe/properties/maxposition">MaxPosition</a> property, you can limit the controllable range. If you specify 0, there is no limit.

Only valid if $TRUE is specified for the <a href="/package/extension4/splitterframe/properties/resize">Resize</a> property.
Setting the <a href="/package/extension4/splitterframe/properties/splitposition">SplitPosition</a> property with a script does not limit the value. 