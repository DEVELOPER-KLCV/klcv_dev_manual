---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetColItemData Method
nav_order: 81
permalink: /package/extension5/sspread/methods/SetColItemData
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetColItemData(<b>col</b>, <b>value</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>value</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    SetColItemData(1, 1001);
    SetColItemData(2, 1002);
    SetColItemData(3, 1003);
    
    Function OnClicked(e) {
        MessageBox(str(GetColItemData(e.Col)) + " is clicked");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/CellTag">CellTag</a> property<br><a href="/package/extension5/sspread/methods/GetColItemData">GetColItemData</a>, <a href="/package/extension5/sspread/methods/GetRowItemData">GetRowItemData</a>, <a href="/package/extension5/sspread/methods/SetRowItemData">SetRowItemData</a> methods</td>
  </tr>
</table>
