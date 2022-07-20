---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetCellSpan Method
nav_order: 35
permalink: /package/extension5/sspread/methods/getcellspan
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Refers to the cell merge status. <br><br>You can check whether the specified cell is included in the merged cell. If included, you can get the column and row numbers for that anchor cell, and the number of columns and rows in the merged cell.<br><br>Use the <a href="/package/extension5/sspread/methods/addcellspan">AddCellSpan</a> method to merge cells. <br> Use the <a href="/package/extension5/sspread/methods/removecellspan">RemoveCellSpan</a> method to unmerge cells.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetCellSpan(<b>col</b>, <b>row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Number object with the following child objects<br><style type="text/css">
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
    <td class="tg-ihln">ColAnchor</td>
    <td class="tg-0lax">Anchor cell column number</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">RowAnchor</td>
    <td class="tg-0lax">Anchor cell row number</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">NumCols</td>
    <td class="tg-0lax">Number of columns in merged cell</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">NumRows</td>
    <td class="tg-0lax">Number of rows in merged cell</td>
  </tr>
</tbody>
</table>
<br>The Value property returns information about the specified cell with the following values:<br>
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-z50u">Value</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$GetCellSpanNo</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Not included in merged cells</td>
  </tr>
  <tr>
    <td class="tg-0lax">$GetCellSpanYes</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Included in the merged cell</td>
  </tr>
  <tr>
    <td class="tg-0lax">$GetCellSpanAnchor</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Corresponds to the anchor cell of the merged cell</td>
  </tr>
</tbody>
</table>
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td>Column number of the referenced cell</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number of the referenced cell</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
   AddCellSpan(2, 3, 4, 4);
    var span = GetCellSpan(4, 4);
    if (span != $GetCellSpanNo) {
        print(span.ColAnchor, span.RowAnchor, span.NumCols, span.NumRows, "\n");
    }
    RemoveCellSpan(span.ColAnchor, span.RowAnchor);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/addcellspan">AddCellSpan</a>, <a href="/package/extension5/sspread/methods/removecellspan">RemoveCellSpan</a> methods</td>
  </tr>
</table>
