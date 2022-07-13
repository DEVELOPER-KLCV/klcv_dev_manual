---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.CopyRange Method
nav_order: 11
permalink: /package/extension5/sspread/methods/copyrange
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Copies the specified cell block to the specified location.<br><br>The data and formats in the cell block are copied. The copy destination cell will be overwritten with the same range as the copy source cell block.<br><br>Use the <a href="/package/extension5/sspread/methods/copycolrange">CopyColRange</a> method to copy a column range and the <a href="/package/extension5/sspread/methods/copyrowrange">CopyRowRange</a> method to copy a row range. The <a href="/package/extension5/sspread/methods/moverange">MoveRange</a> and <a href="/package/extension5/sspread/methods/swaprange">SwapRange</a> methods can be used to move or swap cell blocks.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">CopyRange(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>, <b>coldest</b>, <b>rowdest</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="6">Arguments</td>
    <td><b>col</b></td>
    <td>Column number of the upper left cell of the copy source block</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number in the upper left cell of the copy source block</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Column number of the lower right cell of the copy source block</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Row number of the lower right cell of the copy source block</td>
  </tr>
  <tr>
    <td><b>coldest</b></td>
    <td>Column number of the upper left cell of the copy destination block</td>
  </tr>
  <tr>
    <td><b>rowdest</b></td>
    <td>Row number in the upper left cell of the copy destination block</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the CopyRange method</td>
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
    
    CopyRange(2, 2, 3, 3, 6, 6);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/clearrange">ClearRange</a>, <a href="/package/extension5/sspread/methods/copycolrange">CopyColRange</a>, <a href="/package/extension5/sspread/methods/copyrowrange">CopyRowRange</a>, <a href="/package/extension5/sspread/methods/moverange">MoveRange</a>, <a href="/package/extension5/sspread/methods/swaprange">SwapRange</a> methods</td>
  </tr>
</table>
