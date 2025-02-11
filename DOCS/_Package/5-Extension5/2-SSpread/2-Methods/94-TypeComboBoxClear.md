---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.TypeComboBoxClear Method
nav_order: 94
permalink: /package/extension5/sspread/methods/typecomboboxclear
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Removes all list items from the combo box cell.<br><br>Only valid for cells with $ CellTypeComboBox (combo box type) set in the CellType property. Use the TypeComboBoxRemoveItem method to remove individual list items</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">TypeComboBoxClear(<b>col, row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td>Combo box cell column number</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Row number of combo box type cell</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/celltype">CellType</a> property<br><a href="/package/extension5/sspread/methods/typecomboboxremoveitem">TypeComboBoxRemoveItem</a> method</td>
  </tr>
</table>
