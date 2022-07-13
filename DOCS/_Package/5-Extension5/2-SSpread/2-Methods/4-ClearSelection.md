---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ClearSelection Method
nav_order: 4
permalink: /package/extension5/sspread/methods/clearselection
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Removes all selected cells on the spreadsheet.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ClearSelection()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the ClearRange method<br><small><span style="color:green">Changed to the following specifications since Ver.5.0.3</span></small></td>
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
    <td colspan="2"><a href="/package/extension5/sspread/methods/addselection">AddSelection</a>, <a href="/package/extension5/sspread/methods/setselection">SetSelection</a> methods</td>
  </tr>
</table>
