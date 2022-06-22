---
layout: default

grand_parent: FlexRow Class
parent: Properties
has_children: false
title: FlexRow.End Property
nav_order: 1
permalink: /package/extension4/flexview/flexrow/properties/end
---
# {{ page.title }}

It becomes $TRUE when the row pointed to by FlexRow exceeds the end.

If the last line is exceeded by the <a href="/package/extension4/flexview/flexrow/methods/movenext">MoveNext</a> method, or if the first line is exceeded by the <a href="/package/extension4/flexview/flexrow/methods/moveprev">MovePrev</a> method, it will be $TRUE.

Also, if the method that gets the FlexRow object doesn't find the row to point to, it will be $TRUE.

Even if the End property is $TRUE, you can still call the <a href="/package/extension4/flexview/flexrow/methods/movenext">MoveNext</a>  and <a href="/package/extension4/flexview/flexrow/methods/moveprev">MovePrev</a> methods. For example, you can do the following to find the last row:

```
var row = FlexView1.GetRow();
while( !row.End ) {
    row.MoveNext();
}
row.MovePrev();
```

Notes: This sample is inefficient because it is written for the purpose of explaining the End property. Calling <a href="/package/extension4/flexview/methods/getrow">FlexView.GetRow</a> (-1) is faster to point to the last row.

If the <a href="/package/extension4/flexview/flexrow/properties/invalidstate">InvalidState</a> property is $TRUE, referencing the End property raises the exception EXT-12.