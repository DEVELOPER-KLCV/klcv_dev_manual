---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetCellPos Method
nav_order: 34
permalink: /package/extension5/sspread/methods/GetCellPos
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetCellPos(<b>col</b>, <b>row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
   var ret = GetCellPos(1, 1);
    if (ret == $TRUE) {
        MessageBox(strf("X coordinate:%1 Y coordinate:%2", ret.X, ret.Y));
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/GetCelFromScreenCoord">GetCelFromScreenCoord</a> method</td>
  </tr>
</table>
