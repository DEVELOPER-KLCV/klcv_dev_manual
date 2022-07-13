---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.CopyRowRange Method
nav_order: 12
permalink: /package/extension5/sspread/methods/copyrowrange
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Copies the specified row range to the specified position.<br><br>The row range data and formatting are copied. The copy destination row will be overwritten with the same number of rows as the row range to be copied.<br><br>Use the <a href="/package/extension5/sspread/methods/copyrange">CopyRange</a> method to copy a range of cells and the <a href="/package/extension5/sspread/methods/copycolrange">CopyColRange</a> method to copy a range of columns. You can move or swap row ranges using the <a href="/package/extension5/sspread/methods/moverowrange">MoveRowRange</a> and SwapRowRange methods.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">CopyRowRange(<b>row</b>, <b>row2</b>, <b>rowdest</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>row</b></td>
    <td>The last row number of the row range to copy</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Row number to copy to the row range</td>
  </tr>
  <tr>
    <td><b>rowdest</b></td>
    <td>Row number to copy to the row range</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the CopyRowRange method</td>
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
    
    CopyRowRange(2, 3, 6);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/copycolrange">CopyColRange</a>, <a href="/package/extension5/sspread/methods/copyrange">CopyRange</a>, <a href="/package/extension5/sspread/methods/movecolrange">MoveColRange</a>, <a href="/package/extension5/sspread/methods/moverowrange">MoveRowRange</a>, <a href="/package/extension5/sspread/methods/swapcolrange">SwapColRange</a>, <a href="/package/extension5/sspread/methods/swaprowrange">SwapRowRange</a> methods</td>
  </tr>
</table>
