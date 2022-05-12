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
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetMultiSelItem(<b>prev</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>prev</td>
    <td></td>
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
