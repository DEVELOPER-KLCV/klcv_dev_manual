---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SwapRowRange Method
nav_order: 93
permalink: /package/extension5/sspread/methods/swaprowrange
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Swaps the specified row range with another row range. <br><br>Swaps the data and format of the row range. The number of rows to be replaced is the same as the range of rows to be replaced.<br><br>Use the <a href="/package/extension5/sspread/methods/swaprange">SwapRange</a>  method to swap cell ranges and the <a href="/package/extension5/sspread/methods/swapcolrange">SwapColRange</a> method to swap column ranges.<br> The row range can be copied or moved using the <a href="/package/extension5/sspread/methods/copyrowrange">CopyRowRange</a> and <a href="/package/extension5/sspread/methods/movecolrange">MoveColRange</a> methods.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SwapRowRange(<b>row, row2, rowdest</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>row</b></td>
    <td>Row number at the beginning of the row range of the swap source</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>The last row number in the row range to be swapped</td>
  </tr>
  <tr>
    <td><b>rowdest</b></td>
    <td>Row number at the beginning of the row range of the swap destination</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the SwapRowRange method</td>
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
    Row = 6;
    Row2 = 8;
    Text = "sample2";
    BackColor = $RED;
    BlockMode = $FALSE;
    
    SwapRowRange(2, 3, 6);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/copycolrange">CopyColRange</a>, <a href="/package/extension5/sspread/methods/copyrowrange">CopyRowRange</a>, <a href="/package/extension5/sspread/methods/movecolrange">MoveColRange</a>, <a href="/package/extension5/sspread/methods/moverowrange">MoveRowRange</a>, <a href="/package/extension5/sspread/methods/swapcolrange">SwapColRange</a>, <a href="/package/extension5/sspread/methods/swaprange">SwapRange</a> methods</td>
  </tr>
</table>
