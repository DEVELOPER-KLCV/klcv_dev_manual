---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.SortKeyOrder Property
nav_order: 125
permalink: /package/extension5/sspread/properties/sortkeyorder
---
# {{ page.title }}

Set the sort order (ascending / descending).

This property is an <a href="package/extension5/sspread/#index-property-">Index Property</a>. For the index, specify the priority of the sort key (from 0 to 255, the smaller the higher priority).

Specify the following values. The initial value is $SortKeyOrderAscending.

| Constant                | Value | Description      |
|-------------------------|:-----:|------------------|
| $SortKeyOrderNone       |   0   | No sorting       |
| $SortKeyOrderAscending  |   1   | Ascending order  |
| $SortKeyOrderDescending |   2   | Descending order |

Use this property and the <a href="/package/extension5/sspread/properties/sortkeyorder">SortKeyOrder</a> property to prepare the information you need for sorting.

By making the index (priority) of the SortKey property and SortKeyOrder property the same, you can set the combination of the row / column number used as the sort key and the sort order (ascending / descending order).

The actual sorting is done by calling the <a href="/package/extension5/sspread/methods/sort">Sort</a> method.

Related Items<br>
<a href="/package/extension5/sspread/properties/sortkeyorder">SortKeyOrder</a> property<br>
<a href="/package/extension5/sspread/methods/sort">Sort</a> method

Example of usage<br>
```
SortKey (0) = 2; / * 1st key 2nd column * /
SortKey (1) = 3; / * 2nd key , 3rd column * /
SortKey(2) = 4; /* 3rd key 4th column * /
SortKeyOrder (0) = $ SortKeyOrderAscending;   / * 1st key ascending order * /
SortKeyOrder (1) = $ SortKeyOrderDescending; / * 2nd key descending order * /
SortKeyOrder(2) = $SortKeyOrderDescending; /* 3rd key descending order */
Sort(1, -1, 4 , -1, $SortByRow); /* Sort all rows in columns 1-4 */
```

Related Items<br>
<a href="/package/extension5/sspread/properties/sortkeyorder">SortKeyOrder</a> property<br>
<a href="/package/extension5/sspread/methods/sort">Sort</a> method