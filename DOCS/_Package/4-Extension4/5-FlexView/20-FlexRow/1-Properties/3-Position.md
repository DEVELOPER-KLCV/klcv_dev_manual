---
layout: default

grand_parent: FlexRow Class
parent: Properties
has_children: false
title: FlexRow.Position Property
nav_order: 3
permalink: /package/extension4/flexview/flexrow/properties/position
---
# {{ page.title }}

Indicates the line number currently pointing.

The line number is the line number at the time you refer to the Position property. After getting the FlexRow object, the row numbers may change due to FlexView row operations.

If the <a href="/package/extension4/flexview/flexrow/properties/invalidstate">InvalidState</a> property is $TRUE, referencing the Position property raises the exception EXT-12.

If <a href="/package/extension4/flexview/flexrow/methods/moveprev">MovePrev</a> points before the first line, it will be FlexView.PrevEndPosition (-900).

If <a href="/package/extension4/flexview/flexrow/methods/movenext">MoveNext</a> points to the next in the last row, it will be FlexView.NextEndPosition (-901).