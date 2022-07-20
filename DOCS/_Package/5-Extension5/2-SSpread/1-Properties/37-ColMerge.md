---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ColMerge Property
nav_order: 37
permalink: /package/extension5/sspread/properties/colmerge
---
# {{ page.title }}

Set whether to merge (group) cells with the same contents in a column as one cell that spans multiple rows.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> property to specify the target column.

Specify the following values. The initial value is $MergeNone.

| Constant         | Value | Description                                                                                                                        |
|------------------|:-----:|------------------------------------------------------------------------------------------------------------------------------------|
| $MergeNone       |   0   | Do not merge                                                                                                                       |
| $MergeAlways     |   1   | Always merge <br> If cells with the same content are consecutive, they will always be merged.                                      |
| $MergeRestricted |   2   | Restrict merge <br> If cells with the same contents are consecutive, they will be merged only if the cells to the left are merged. |

Operation Example

<a href="/img/package/Ext5-SSpread-ColMerge.PNG" target="_blank">
<img src="/img/package/Ext5-SSpread-ColMerge.PNG" alt="login image">
</a>

For the merged cells, the settings of the upper left cell (background color, etc.) are enabled.

The data in the other merged cells will only be hidden and not deleted.

Row merging is set in the <a href="/package/extension5/sspread/properties/rowmerge">RowMerge</a> property.

Example of usage<br>
```
Col = 1;
ColMerge = $MergeAlways;
Col = 2;
ColMerge = $MergeRestricted;
```

Related Item<br>
<a href="/package/extension5/sspread/properties/rowmerge">RowMerge</a> property