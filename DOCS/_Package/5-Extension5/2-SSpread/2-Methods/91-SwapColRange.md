---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SwapColRange Method
nav_order: 91
permalink: /package/extension5/sspread/methods/swapcolrange
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Swaps the specified column range with another column range.<br><br>Swap the data and format of the column range. The number of columns to be replaced is the same as the range of columns to be replaced.<br><br>Use the <a href="/package/extension5/sspread/methods/swaprange">SwapRange</a> method to swap cell ranges and the <a href="/package/extension5/sspread/methods/swaprowrange">SwapRowRange</a> method to swap rows. The column range can be copied or moved using the <a href="/package/extension5/sspread/methods/copyrowrange">CopyRowRange</a> and <a href="/package/extension5/sspread/methods/movecolrange">MoveColRange</a> methods.</td>
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
    <td>Column number at the beginning of the column range of the swap source</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Last column number in the source column range</td>
  </tr>
  <tr>
    <td><b>coldest</b></td>
    <td>Column number at the beginning of the column range of the swap destination</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the SwapColRange method</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/methods/copycolrange">CopyColRange</a>, <a href="/package/extension5/sspread/methods/copyrowrange">CopyRowRange</a>, <a href="/package/extension5/sspread/methods/movecolrange">MoveColRange</a>, <a href="/package/extension5/sspread/methods/moverowrange">MoveRowRange</a>, <a href="/package/extension5/sspread/methods/swaprange">SwapRange</a>, <a href="/package/extension5/sspread/methods/swaprowrange">SwapRowRange</a> methods</td>
  </tr>
</table>
