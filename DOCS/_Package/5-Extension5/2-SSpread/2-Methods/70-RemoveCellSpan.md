---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.RemoveCellSpan Method
nav_order: 70
permalink: /package/extension5/sspread/methods/removecellspan
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Unmerge cells.<br><br>The cell range containing the specified anchor cell is unmerged.<br><br> Use the GetCellSpan method to see the cell merge status. Use the AddCellSpan method to merge cells.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">RemoveCellSpan(<b>col</b>, <b>row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td>Column number of anchor cell to be unmerged</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number of the anchor cell to be unmerged</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/methods/addcellspan">AddCellSpan</a>, <a href="/package/extension5/sspread/methods/getcellspan">GetCellSpan</a> method</td>
  </tr>
</table>
