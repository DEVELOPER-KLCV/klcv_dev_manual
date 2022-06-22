---
layout: default

grand_parent: FlexRow Class
parent: Properties
has_children: false
title: FlexRow.InvalidState Property
nav_order: 2
permalink: /package/extension4/flexview/flexrow/properties/invalidstate
---
# {{ page.title }}

FlexRow will be $TRUE if it no longer points to any row.

If the InvalidState property is $TRUE, an exception will occur if you move a row with <a href="/package/extension4/flexview/flexrow/methods/movenext">MoveNext</a>, refer to the <a href="/package/extension4/flexview/flexrow/properties/position">Postion</a> property, or perform any other operation that depends on the row you are pointing to.

The InvalidState property is set to $TRUE by the following operation.
-When deleting the row pointed to by the FlexRow object.
-When the <a href="/package/extension4/flexview">FlexView</a> object is deleted.