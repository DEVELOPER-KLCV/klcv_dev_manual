---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetFirstValidCell Method
nav_order: 40
permalink: /package/extension5/sspread/methods/getfirstvalidcell
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the column number and row number of the first valid cell.<br><br>You can look up the first valid cell, excluding hidden cells, such as when the row height or column width is 0.<br><br>If the <a href="/package/extension5/sspread/properties/editmodepermanent">EditModePermanent</a> property is $TRUE, locked cells, label-type, and picture-type cells are not treated as valid cells.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetFirstValidCell()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Record object with the following child objects<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-ihln{font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Type</th>
    <th class="tg-z50u">Name</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Col</td>
    <td class="tg-0lax">Column number of the first valid cell</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Row</td>
    <td class="tg-0lax">Row number of the first valid cell</td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the GetFirstValidCell method

</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var ret = GetFirstValidCell();
    MessageBox(strf("The first valid cell is(%1,%2)", ret.Col, ret.Row));
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/colwidth">ColWidth</a>, <a href="/package/extension5/sspread/properties/editmodepermanent">EditModePermanent</a>, <a href="/package/extension5/sspread/properties/lock">Lock</a>, <a href="/package/extension5/sspread/properties/rowheight">RowHeight</a> properties<br><a href="/package/extension5/sspread/methods/getlastvalidcell">GetLastValidCell</a> method</td>
  </tr>
</table>
