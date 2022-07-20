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
    <td colspan="2">Replaces the data and format of the specified cell range with other cell ranges.<br><br>Swap the data and formats in the cell blocks. The cell to be replaced will be replaced in the same range as the cell block to be replaced.<br><br>Use the <a href="/package/extension5/sspread/methods/swapcolrange">SwapColRange</a> method to swap column ranges and the <a href="/package/extension5/sspread/methods/swaprowrange">SwapRowRange</a> method to swap row ranges. Cell blocks can be copied and moved using the <a href="/package/extension5/sspread/methods/copyrange">CopyRange</a> and <a href="/package/extension5/sspread/methods/moverange">MoveRange</a> methods.</td>
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
    <td>Column number of the upper left cell of the cell range of the replacement source</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number of the upper left cell of the cell range of the replacement source</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Column number of the lower right cell of the cell range of the replacement source</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Row number of the lower right cell of the cell range of the replacement source</td>
  </tr>
  <tr>
    <td><b>coldest</b></td>
    <td>Column number of the upper left cell of the replacement destination cell range</td>
  </tr>
  <tr>
    <td><b>rowdest</b></td>
    <td>The row number of the upper left cell of the cell range to be replaced</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the SwapRange method</td>
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
