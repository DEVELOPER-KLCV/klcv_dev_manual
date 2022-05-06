---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.AddCellSpan Method
nav_order: 1
permalink: /package/extension5/sspread/methods/addcellspan
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">AddCellSpan(<b>col</b>, <b>row</b>, <b>numcols</b>, <b>numrows</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td><b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>numcols</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>numrows</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td></td>
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
    <td colspan="2"><a href="/package/extension5/sspread/methods/getcellspan">GetCellSpan</a>, <a href="/package/extension5/sspread/methods/removecellspan">RemoveCellSpan</a> methods</td>
  </tr>
</table>
