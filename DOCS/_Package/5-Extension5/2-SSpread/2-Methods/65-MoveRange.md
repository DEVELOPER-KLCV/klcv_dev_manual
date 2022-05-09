---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.MoveRange Method
nav_order: 65
permalink: /package/extension5/sspread/methods/MoveRange
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">MoveRange(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>, <b>coldest</b>, <b>rowdest</b>)</td>
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
    BlockMode = $FALSE;
    
    MoveRange(2, 2, 3, 3, 6, 6);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/clearrange">ClearRange</a>, <a href="/package/extension5/sspread/methods/copyrange">CopyRange</a>, <a href="/package/extension5/sspread/methods/movecolrange">MoveColRange</a>, <a href="/package/extension5/sspread/methods/moverowrange">MoveRowRange</a>, <a href="/package/extension5/sspread/methods/swaprange">SwapRange</a> methods</td>
  </tr>
</table>
