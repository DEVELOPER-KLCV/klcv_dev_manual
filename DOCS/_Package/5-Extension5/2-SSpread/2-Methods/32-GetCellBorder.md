---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetCellBorder Method
nav_order: 32
permalink: /package/extension5/sspread/methods/getcellborder
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetCellBorder(<b>col</b>, <b>row</b>, <b>index</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>index</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var ret = GetCellBorder(1, 1, $CellBorderIndexLeft);
    var style = "";
    switch (ret.Style){
        case $CellBorderStyleDefault:
            style = "No ruled lines";
            break;
        case $CellBorderStyleSolid:
            style = "Solid line";
            break;
        default:
            style = "Others";
            break;
    }
    MessageBox("The ruled line on the left side of (1, 1)「" + style + "」で、colour is" + str(ret.Color));
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/setcellborder">SetCellBorder</a> method</td>
  </tr>
</table>
