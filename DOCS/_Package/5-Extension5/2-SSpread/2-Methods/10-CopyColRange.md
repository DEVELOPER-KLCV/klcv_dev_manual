---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.CopyColRange Method
nav_order: 10
permalink: /package/extension5/sspread/methods/copycolrange
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Copies the specified column range to the specified position.<br><br>The data and format of the column range is copied. The destination column will be overwritten with the same number of columns as the column range to be copied.<br><br>Use the <a href="/package/extension5/sspread/methods/copyrange">CopyRange</a> method to copy a range of cells and the <a href="/package/extension5/sspread/methods/copyrowrange">CopyRowRange</a> method to copy a range of rows. The <a href="/package/extension5/sspread/methods/movecolrange">MoveColRange</a> and <a href="/package/extension5/sspread/methods/swapcolrange">SwapColRange</a> methods can be used to move or swap column ranges.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">CopyColRange(<b>col</b>, <b>col2</b>, <b>coldest</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>col</b></td>
    <td>First column number of the range to copy</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Last column number in the range to copy</td>
  </tr>
  <tr>
    <td><b>coldest</b></td>
    <td>Column number to copy to the column range</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the CopyColRange method</td>
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
    
    CopyColRange(2, 3, 6);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/copyrange">CopyRange</a>, <a href="/package/extension5/sspread/methods/copyrowrange">CopyRowRange</a>, <a href="/package/extension5/sspread/methods/movecolrange">MoveColRange</a>, <a href="/package/extension5/sspread/methods/moverowrange">MoveRowRange</a>, <a href="/package/extension5/sspread/methods/swapcolrange">SwapColRange</a>, <a href="/package/extension5/sspread/methods/swaprowrange">SwapRowRange</a> methods</td>
  </tr>
</table>
