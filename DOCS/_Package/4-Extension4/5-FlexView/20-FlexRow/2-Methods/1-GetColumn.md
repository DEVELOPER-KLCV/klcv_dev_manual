---
layout: default

grand_parent: FlexRow Class
parent: Methods
has_children: false
title: FlexRow.GetColumn Method
nav_order: 1
permalink: /package/extension4/flexview/flexrow/methods/getcolumn
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var col = row.GetColumn( <b>pos</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>pos</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-12</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var row = FlexView1.GetRow();
    var key = null;
    var sum = 0;
    while (!row.End) {
        var col = row.GetColumn(1);
        col.BgColor = $STD;
        row.MoveNext();
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>