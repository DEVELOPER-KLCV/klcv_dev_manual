---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetLastValidCell Method
nav_order: 43
permalink: /package/extension5/sspread/methods/getlastvalidcell
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetLastValidCell()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var ret = GetLastValidCell();
    MessageBox(strf("The last valid cell is(%1,%2)", ret.Col, ret.Row));
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/colwidth">ColWidth</a>, <a href="/package/extension5/sspread/properties/editmodepermanent">EditModePermanent</a>, <a href="/package/extension5/sspread/properties/lock">Lock</a>, <a href="/package/extension5/sspread/properties/rowheight">RowHeight</a> properties<br><a href="/package/extension5/sspread/methods/getfirstvalidcell">GetFirstValidCell</a> method</td>
  </tr>
</table>
