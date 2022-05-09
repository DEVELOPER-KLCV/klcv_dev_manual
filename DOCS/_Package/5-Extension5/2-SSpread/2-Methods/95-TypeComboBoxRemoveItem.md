---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.TypeComboBoxRemoveItem Method
nav_order: 95
permalink: /package/extension5/sspread/methods/TypeComboBoxRemoveItem
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">TypeComboBoxRemoveItem(<b>col, row, index</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td></td>
  </tr>
  <tr>
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
    Col = 1;
    Row = 1;
    CellType = $CellTypeComboBox;
    TypeComboBoxList = "Remove All \tItem 1\tItem 2\tItem 3\tItem 4\tItem 5";
    
    Function OnComboCloseUp(e) {
        if (e.SelChange == 0) {
            TypeComboBoxClear(e.Col, e.Row);
        } else if (e.SelChange > 0) {
            TypeComboBoxRemoveItem(e.Col, e.Row, e.SelChange);
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/celltype">CellType</a> property<br><a href="/package/extension5/sspread/methods/TypeComboBoxClear">TypeComboBoxClear</a> method</td>
  </tr>
</table>
