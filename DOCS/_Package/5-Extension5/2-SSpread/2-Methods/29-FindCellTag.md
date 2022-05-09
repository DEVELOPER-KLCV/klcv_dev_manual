---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.FindCellTag Method
nav_order: 29
permalink: /package/extension5/sspread/methods/FindCellTag
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var rec = FindCellTag(<b>tag</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>tag</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var rec = Spread1.FindCellTag("Summary items");
    if (rec != null) {
    Spread1.Col = rec.Col;
    Spread1.Row = rec.Row;
    Spread1.Text = data;
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/celltag">CellTag</a> property</td>
  </tr>
</table>
