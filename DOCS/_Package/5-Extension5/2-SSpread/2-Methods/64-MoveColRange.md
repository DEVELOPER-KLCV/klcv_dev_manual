---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.MoveColRange Method
nav_order: 64
permalink: /package/extension5/sspread/methods/movecolrange
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Moves the specified column range to the specified position.<br><br>Moves the data and format of the column range. The destination column will be overwritten with the same number of columns as the range of columns to move.<br><br>Use the <a href="/package/extension5/sspread/methods/moverange">MoveRange</a> method to move the cell range and the <a href="/package/extension5/sspread/methods/moverowrange">MoveRowRange</a> method to move the row range. The <a href="/package/extension5/sspread/methods/copycolrange">CopyColRange</a> and <a href="/package/extension5/sspread/methods/swapcolrange">SwapColRange</a> methods can be used to copy or swap column ranges.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">MoveColRange(<b>col</b>, <b>col2</b>, <b>coldest</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>col</b></td>
    <td>First column number of the range to move</td>
  </tr>  
  <tr>
    <td><b>col2</b></td>
    <td>Last column number of the range to move</td>
  </tr>  
  <tr>
    <td><b>coldest</b></td>
    <td>Column number of the moved column range</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the MoveColRange method</td>
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
    
    MoveColRange(2, 3, 6);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/copycolrange">CopyColRange</a>, <a href="/package/extension5/sspread/methods/copyrowrange">CopyRowRange</a>, <a href="/package/extension5/sspread/methods/moverange">MoveRange</a>, <a href="/package/extension5/sspread/methods/moverowrange">MoveRowRange</a>, <a href="/package/extension5/sspread/methods/swapcolrange">SwapColRange</a>, <a href="/package/extension5/sspread/methods/swaprowrange">SwapRowRange</a> methods</td>
  </tr>
</table>
