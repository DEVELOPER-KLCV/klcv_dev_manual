---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.RowMerge Property
nav_order: 95
permalink: /package/extension5/sspread/properties/rowmerge
---
# {{ page.title }}

Set whether to merge (group) cells with the same contents in a row as one cell that spans multiple columns.

Before setting this property, use the <a href="/package/extension5/sspread/properties/row">Row</a> property to specify the desired row.

Specify the following values. The initial value is $MergeNone

| Constant         | Value | Description                                                                                                                         |
|------------------|:-----:|-------------------------------------------------------------------------------------------------------------------------------------|
| $MergeNone       |   0   | Do not merge                                                                                                                        |
| $MergeAlways     |   1   | Always merge <br> Whenever cells with the same content are consecutive, they are merged.                                            |
| $MergeRestricted |   2   | Restricted merge <br> If cells with the same contents are consecutive, they will be merged only if the cells above them are merged. |

Operation Example<br>

<a href="/img/Package/Ext5-SSpread-RowMerge.PNG" target="_blank">
<img src="/img/Package/Ext5-SSpread-RowMerge.PNG" alt="login image">
</a>

For the merged cells, the settings of the upper left cell (background color, etc.) are valid.

The data in the other merged cells is only hidden and not deleted.

Column merging is set with the <a href="/package/extension5/sspread/properties/colmerge">ColMerge</a> property.

Example of usage<br>
```
Row = 1;
RowMerge = $MergeAlways;
Row = 2;
RowMerge = $MergeRestricted;
``` 

Related Item<br>
<a href="/package/extension5/sspread/properties/colmerge">ColMerge</a> property 

