---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetCellBorder Method
nav_order: 80
permalink: /package/extension5/sspread/methods/SetCellBorder
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetCellBorder(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>, <b>index</b>, <b>color</b>, <b>style</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
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
    <td><b>index</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>color</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>style</b></td>
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
    SetCellBorder(2, 2, 2, 2, $CellBorderIndexOutline, $RED, $CellBorderStyleSolid);
    SetCellBorder(2, 4, 3, 6, $CellBorderIndexOutline, $BLUE, $CellBorderStyleDot);
    SetCellBorder(4, 2, 4, 6, $CellBorderIndexRight + $CellBorderIndexTop, $GREEN, $CellBorderStyleFineSolid);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/GetCellBorder">GetCellBorder</a> method</td>
  </tr>
</table>
