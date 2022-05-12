---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SwapRange Method
nav_order: 92
permalink: /package/extension5/sspread/methods/swaprange
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SwapRange(<b>col, col2, row2, coldest, rowdest</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="6">Arguments</td>
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
    <td><b>coldest</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>rowdest</b></td>
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
    BlockMode = $TRUE;
    Col = 2;
    Row = 2;
    Col2 = 4;
    Row2 = 4;
    Text = "sample";
    BackColor = $GREEN;
    Col = 6;
    Row = 6;
    Col2 = 8;
    Row2 = 8;
    Text = "sample2";
    BackColor = $RED;
    BlockMode = $FALSE;
    
    SwapRange(2, 2, 3, 3, 6, 6);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/clearrange">ClearRange</a>, <a href="/package/extension5/sspread/methods/copyrange">CopyRange</a>, <a href="/package/extension5/sspread/methods/moverange">MoveRange</a>, <a href="/package/extension5/sspread/methods/swapcolrange">SwapColRange</a>, <a href="/package/extension5/sspread/methods/swaprowrange">SwapRowRange</a> methods</td>
  </tr>
</table>
