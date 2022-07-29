---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeHAlign Property
nav_order: 178
permalink: /package/extension5/sspread/properties/typehalign
---
# {{ page.title }}

Set the horizontal alignment within the cell.

Only valid for cells with the following <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
<br>$CellTypeDate (date type)
<br>$CellTypeEdit (character type)
<br>$CellTypePic (mask type)
<br>$CellTypeStaticText (label type)
<br>$CellTypeTime (time type)
<br>$CellTypeComboBox (combo box type)
<br>$CellTypePicture (picture type)
<br>$CellTypeCheckBox (checkbox type)
<br>$CellTypeCurrency (currency type)
<br>$CellTypeNumber (numeric type)
<br>$CellTypePercent (percent type)
<br>$CellTypeScientific (exponential type)

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.


Specify the following values.
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-2m49{background-color:#D9D9D9;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05">Constant</th>
    <th class="tg-2m49">Value</th>
    <th class="tg-xt05">Explanation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$ TypeHAlignLeft</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Left justified</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeHAlignRight</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Right justified</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeHAlignCenter</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Centered</td>
  </tr>
</tbody>
</table>

The initial value depends on the data type of the cell.
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Currency type, Numerical type, Percentage type, Exponential type</th>
    <th class="tg-0lax">$ TypeHAlignRight</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Label type cells for column headers and row headers</td>
    <td class="tg-0lax">$ TypeHAlignCenter</td>
  </tr>
  <tr>
    <td class="tg-0lax">Other than above</td>
    <td class="tg-0lax">$ TypeHAlignLeft</td>
  </tr>
</tbody>
</table>

The vertical alignment is set with the <a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a> property.
<br>The placement of command button cell types is set with the <a href="/package/extension5/sspread/properties/typebuttonalign">TypeButtonAlign</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for for each data type cell.
<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-combo-box-type-cells">Notes on property inheritance of combo box type cells</a>
<br><a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-label-type-cells">Notes on property inheritance of label type cells</a>

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeStaticText;
TypeHAlign = $ TypeHAlignRight;
TypeVAlign = $ TypeVAlignBottom;
Text = "sample";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeNumber;
TypeHAlign = $ TypeHAlignLeft;
TypeVAlign = $ TypeVAlignCenter;
Value = 12345;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typebuttonalign">TypeButtonAlign</a> ,<a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a> property
