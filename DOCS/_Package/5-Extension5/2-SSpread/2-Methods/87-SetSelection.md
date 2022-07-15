---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetSelection Method
nav_order: 87
permalink: /package/extension5/sspread/methods/setselection
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Select the cell block on the spreadsheet.<br><br> Refer to the <a href="/package/extension5/sspread/properties/selblockcol">SelBlockCol</a>, <a href="/package/extension5/sspread/properties/selblockcol2">SelBlockCol2</a>, <a href="/package/extension5/sspread/properties/selblockrow">SelBlockRow</a> and <a href="/package/extension5/sspread/properties/selblockrow2">SelBlockRow2</a> properties to get the selected cell block.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetSelection(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td><b>col</b></td>
    <td>The leftmost column number of the cell block to select</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number at the top of the cell block to select</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Rightmost column number of the cell block to select</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Row number at the bottom of the cell block to select</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the SetSelection method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    SetSelection(2, 3, 4, 5);
    print(SelBlockCol, SelBlockRow, SelBlockCol2, SelBlockRow2, "\n");
    ClearSelection();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/selblockcol">SelBlockCol</a>, <a href="/package/extension5/sspread/properties/selblockcol2">SelBlockCol2</a>, <a href="/package/extension5/sspread/properties/selblockrow">SelBlockRow</a>, <a href="/package/extension5/sspread/properties/selblockrow2">SelBlockRow2</a> properties<br><a href="/package/extension5/sspread/methods/clearselection">ClearSelection</a> method</td>
  </tr>
</table>
