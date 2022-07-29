---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeComboBoxWidth Property
nav_order: 156
permalink: /package/extension5/sspread/properties/typecomboboxwidth
---
# {{ page.title }}

Set the width of the list in the combo box cell.

Only valid for cells with $CellTypeComboBox (combo box type) set in the CellT <a href="/package/extension5/sspread/properties/celltype">CellType</a>ype property.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the following values. The initial value is 0.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-266k{background-color:#9b9b9b;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-266k">Value</th>
    <th class="tg-266k">List Width</th>
    <th class="tg-266k">List display position</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">0</td>
    <td class="tg-0pky">Same as cell width</td>
    <td class="tg-0pky">-</td>
  </tr>
  <tr>
    <td class="tg-0pky">1</td>
    <td class="tg-0pky">Fit to the longest list item</td>
    <td class="tg-0pky" rowspan="2">Align to the right edge of the cell if the width of the cell is greater<br>Align to the left edge of the cell if the list is wider</td>
  </tr>
  <tr>
    <td class="tg-0pky">n ( value greater than 1 )</td>
    <td class="tg-0pky">n pixels</td>
  </tr>
  <tr>
    <td class="tg-0pky">-1</td>
    <td class="tg-0pky">Fit to the longest list item</td>
    <td class="tg-0pky" rowspan="2">Always align to the right edge of the cell</td>
  </tr>
  <tr>
    <td class="tg-0pky">-n ( value less than -1 )</td>
    <td class="tg-0pky">n pixels</td>
  </tr>
</tbody>
</table>

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for combo box cells.

<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-combo-box-type-cells">Notes on property inheritance of combo box type cells</a>

Example of usage<br>
```
Col = 3;
Row = 2;
CellType = $CellTypeComboBox;
TypeComboBoxList = "AAA\tBBB\tCCC";
TypeComboBoxWidth = 100;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeComboBox;
TypeComboBoxWidth = 1;
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typecomboboxlist">TypeComboBoxList</a> properties<br>
