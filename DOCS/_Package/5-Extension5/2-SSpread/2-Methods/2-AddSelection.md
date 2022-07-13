---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.AddSelection Method
nav_order: 2
permalink: /package/extension5/sspread/methods/addselection
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Add a selection of cell blocks.<br><br>Adds a new cell block selection if the user is allowed to select multiple cell blocks (if the <a href="/package/extension5/sspread/properties/allowmutiblocks">AllowMultiBlocks</a> property is $TRUE).<br><br> To get the selected cell block, use the <a href="/package/extension5/sspread/methods/getselection">GetSelection</a> method.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">AddSelection(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td><b>col</b></td>
    <td>Leftmost column number of cell block</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number at the top of the cell block</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Rightmost column number of cell block</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Row number at the bottom of the cell block</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the AddSelection method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    AllowMultiBlocks = $TRUE;
    AddSelection(2, 2, 4, 3);
    AddSelection(1, 5, 5, 5);
    AddSelection(2, 7, 4, 7);
    for (var n = 0; n < SelectionCount; n++) {
        var sel = GetSelection(n);
        print(sel.Col, sel.Row, sel.Col2, sel.Row2, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/allowmutiblocks">AllowMultiBlocks</a> property<br><a href="/package/extension5/sspread/methods/clearselection">ClearSelection</a>, <a href="/package/extension5/sspread/methods/getselection">GetSelection</a> methods</td>
  </tr>
</table>
