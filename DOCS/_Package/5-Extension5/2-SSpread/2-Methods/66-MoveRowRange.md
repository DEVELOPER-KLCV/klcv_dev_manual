---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.MoveRowRange Method
nav_order: 66
permalink: /package/extension5/sspread/methods/moverowrange
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Moves the specified row range to the specified position. <br><br>Moves the data and format of the row range. The destination row will be overwritten with the same number of rows as the range of rows to be moved.<br><br> Use the <a href="/package/extension5/sspread/methods/moverange">MoveRange</a> method to move the cell range and the <a href="/package/extension5/sspread/methods/movecolrange">MoveColRange</a> method to move the column range. Row ranges can be copied or swapped using the <a href="/package/extension5/sspread/methods/copyrowrange">CopyRowRange</a> and <a href="/package/extension5/sspread/methods/swaprowrange">SwapRowRange</a> methods.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">MoveRowRange(<b>row</b>, <b>row2</b>, <b>rowdest</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>row</b></td>
    <td>The first row number of the range to move</td>
  </tr>  
  <tr>
    <td><b>row2</b></td>
    <td>The last row number of the range to move</td>
  </tr>  
  <tr>
    <td><b>rowdest</b></td>
    <td>The row number to which the row range is moved</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the MoveRowRange method</td>
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
    
    MoveRowRange(2, 3, 6);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/copycolrange">CopyColRange</a>, <a href="/package/extension5/sspread/methods/copyrowrange">CopyRowRange</a>, <a href="/package/extension5/sspread/methods/movecolrange">MoveColRange</a>, <a href="/package/extension5/sspread/methods/moverange">MoveRange</a>, <a href="/package/extension5/sspread/methods/swapcolrange">SwapColRange</a>, <a href="/package/extension5/sspread/methods/swaprowrange">SwapRowRange</a> methods</td>
  </tr>
</table>
