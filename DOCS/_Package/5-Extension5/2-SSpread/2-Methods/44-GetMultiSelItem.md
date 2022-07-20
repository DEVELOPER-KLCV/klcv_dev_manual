---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetMultiSelItem Method
nav_order: 44
permalink: /package/extension5/sspread/methods/getmultiselitem
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the number of the selected line in multiple selection mode.<br><br>This is valid only when the <a href="/package/extension5/sspread/properties/operationmode">OperationMode</a> property is $OperationModeMulti (multiple selection mode) and $OperationModeExtended (extended multiple selection mode).<br><br>Call this method repeatedly to find out the numbers of all the selected lines. When examining the first line, specify 0 for the argument <b>prev</b>. When looking at the next line, set the return value of the first call to the argument <b>prev</b>. If there are no more rows selected, -1 is returned.<br><br>The number of selected lines can be obtained with the <a href="/package/extension5/sspread/properties/selectioncount">SelectionCount</a> property. Use the <a href="/package/extension5/sspread/properties/selmodeselected">SelModeSelected</a> property to select a row from the CRS program.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetMultiSelItem(<b>prev</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Selected line number</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>prev</b></td>
    <td>The number of the selected line immediately before (0 to line number)</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    OperationMode = $OperationModeMulti;
    Function OnClicked(e) {
        var prev = GetMultiSelItem(0);
        while (prev >= 0) {
            print(prev, " ");
            prev = GetMultiSelItem(prev);
        }
        print("\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/operationmode">OperationMode</a>, <a href="/package/extension5/sspread/properties/selectioncount">SelectionCount</a>, <a href="/package/extension5/sspread/properties/selmodeselected">SelModeSelected</a> properties</td>
  </tr>
</table>
