---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetSelection Method
nav_order: 48
permalink: /package/extension5/sspread/methods/GetSelection
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetSelection(<b>index</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>index</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/allowmultiblocks">AllowMultiBlocks</a>, <a href="/package/extension5/sspread/properties/selectioncount">SelectionCount</a> property<br><a href="/package/extension5/sspread/methods/AddSelection">AddSelection</a> method</td>
  </tr>
</table>
