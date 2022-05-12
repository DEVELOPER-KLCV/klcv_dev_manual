---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.Sort Method
nav_order: 90
permalink: /package/extension5/sspread/methods/sort
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">Sort(<b>col, row, col2, row2, sortby [, sortkeys, sortkeyorders]</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="7">Arguments</td>
    <td><b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>sortby</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>sortkeys</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>sortkeyorders</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-1</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    /* Example of using SortKey and SortKeyOrder properties */
    SortKey(0) = 2; /* 1st key 2nd column */
    SortKey(1) = 3; /* 2nd key 3rd column */
    SortKey(2) = 4; /* 3rd key 4th column */
    SortKeyOrder(0) = $SortKeyOrderAscending;  /* 1st key ascending order */
    SortKeyOrder(1) = $SortKeyOrderDescending; /* 2nd key descending order */
    SortKeyOrder(2) = $SortKeyOrderDescending; /* 3rd key descending order */
    Sort(1, -1, 4, -1, $SortByRow); /* Sort all rows in columns 1 to 4 */
    
    /* Example of specifying all with arguments (processing content is the same as above) */
    var sortkeys = new Number[3];
    var sortorder = new Number[3];
    sortkeys[0] = 2;
    sortkeys[1] = 3;
    sortkeys[2] = 4;
    sortorder[0] = 1;
    sortorder[1] = 2;
    sortorder[2] = 2;
    Sort(1, -1, 4, -1, $SortByRow, sortkeys, sortorder);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/sortkey">SortKey</a>, <a href="/package/extension5/sspread/properties/sortkeyorder">SortKeyOrder</a> properties</td>
  </tr>
</table>
