---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SwapColRange Method
nav_order: 91
permalink: /package/extension5/sspread/methods/SwapColRange
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SwapColRange(<b>col, col2, coldest</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>coldest</b></td>
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
    Col2 = 8;
    Text = "sample2";
    BackColor = $RED;
    BlockMode = $FALSE;
    
    SwapColRange(2, 3, 6);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/copycolrange">CopyColRange</a>, <a href="/package/extension5/sspread/methods/CopyRowRange">CopyRowRange</a>, <a href="/package/extension5/sspread/methods/MoveColRange">MoveColRange</a>, <a href="/package/extension5/sspread/methods/MoveRowRange">MoveRowRange</a>, <a href="/package/extension5/sspread/methods/SwapRange">SwapRange</a>, <a href="/package/extension5/sspread/methods/SwapRowRange">SwapRowRange</a> methods</td>
  </tr>
</table>
