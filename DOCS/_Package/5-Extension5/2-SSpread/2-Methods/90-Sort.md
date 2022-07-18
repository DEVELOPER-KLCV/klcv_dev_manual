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
    <td colspan="2">Sorts the specified data.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">Sort(<b>col, row, col2, row2, sortby [, sortkeys, sortkeyorders]</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">$TRUE if successful, $FALSE otherwise</td>
  </tr>  
  <tr>
    <td rowspan="7">Arguments</td>
    <td><b>col</b></td>
    <td>First column number in the sort range</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number at the beginning of the sort range</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Last column number in the sort range</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Last row number in the sort range</td>
  </tr>
  <tr>
    <td><b>sortby</b></td>
    <td>Sort type<br>Specify the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-k3us{background-color:#D9D9D9;border-color:inherit;color:#5C5962;font-family:Arial, Helvetica, sans-serif !important;
  text-align:center;vertical-align:top}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-gpky{background-color:#D9D9D9;border-color:inherit;color:#5C5962;text-align:left;vertical-align:top}
.tg .tg-lsj2{background-color:#D9D9D9;border-color:inherit;color:#5C5962;font-family:Arial, Helvetica, sans-serif !important;
  text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-lsj2">Constant</th>
    <th class="tg-k3us">Value</th>
    <th class="tg-gpky">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$SortByRow</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Sort rows</td>
  </tr>
  <tr>
    <td class="tg-0lax">$SortByCol</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Sort columns</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td><b>sortkeys</b></td>
    <td>An array object (optional) that indicates the column / row number to be used as the sort key.</td>
  </tr>
  <tr>
    <td><b>sortkeyorders</b></td>
    <td>An array object that indicates the sort order (optional)<br>Specify the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-k3us{background-color:#D9D9D9;border-color:inherit;color:#5C5962;font-family:Arial, Helvetica, sans-serif !important;
  text-align:center;vertical-align:top}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-6n9o{background-color:#D9D9D9;border-color:inherit;color:#5C5962;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-k3us">Value</th>
    <th class="tg-6n9o">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-baqh">1</td>
    <td class="tg-baqh">Sort in ascending order</td>
  </tr>
  <tr>
    <td class="tg-baqh">2</td>
    <td class="tg-baqh">Sort in descending order</td>
  </tr>
</tbody>
</table><br> 
For <b>sortkeys</b> and <b>sortkeyorders</b>, specify an <a href="/4000/bizBrowserV/6/6-1/">Array Object</a> that has the information required for sorting. The smaller the index of the array, the higher the priority of the sort keys.

By making the indexes the same, the combination of the row / column number can be set to be the key for sorting and the sorting order (ascending / descending order).

If <b>sortkeys</b> and <b>sortkeyorders</b> are omitted, the values of the <a href="/package/extension5/sspread/properties/sortkey">SortKey</a> property and <a href="/package/extension5/sspread/properties/sortkeyorder">SortKeyOrder</a> property are used.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-1</td>
    <td>The argument of Sort is invalid</td>
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
