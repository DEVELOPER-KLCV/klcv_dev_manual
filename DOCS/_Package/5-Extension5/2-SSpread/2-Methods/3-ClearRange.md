---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ClearRange Method
nav_order: 3
permalink: /package/extension5/sspread/methods/clearrange
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify a range to erase the data.<br><br>Remove data, formulas from cells, columns, rows, cell blocks, or the entire spreadsheet.<br><br>By specifying the argument <b>dataonly</b>, you can select whether to initialize the format (font, background color, text color, cell type, etc.) or delete only the data and formula.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ClearRange(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>, <b>dataonly</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="5">Arguments</td>
    <td><b>col</b></td>
    <td>Column number of the upper left cell of the cell block to be erased</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number of the upper left cell of the cell block to be erased</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Column number of the lower right cell of the cell block to be erased</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Row number of the lower right cell of the cell block to be erased</td>
  </tr>
  <tr>
    <td><b>dataonly</b></td>
    <td>$TRUE to erase only data, $FALSE to erase formatted data</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the ClearRange method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    BlockMode = $TRUE;
    Col = 2;
    Row = 2;
    Col2 = 5;
    Row2 = 5;
    Text = "sample";
    BackColor = $GREEN;
    BlockMode = $FALSE;
    
    ClearRange(2, 2, 3, 3, $TRUE);
    ClearRange(4, 4, 5, 5, $FALSE);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/copyrange">CopyRange</a>, <a href="/package/extension5/sspread/methods/moverange">MoveRange</a>, <a href="/package/extension5/sspread/methods/reset">Reset</a>, <a href="/package/extension5/sspread/methods/swaprange">SwapRange</a> methods</td>
  </tr>
</table>
