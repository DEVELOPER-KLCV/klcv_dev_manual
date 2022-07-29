---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeVAlign Property
nav_order: 218
permalink: /package/extension5/sspread/properties/typevalign
---
# {{ page.title }}
Set the vertical alignment within the cell.

Only valid for cells with the following values ​​set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
<br>$ CellTypeDate (date type) 
<br>$ CellTypeEdit (character type)
<br>$ CellTypePic (mask type)
<br>$ CellTypeStaticText (label type)
<br>$ CellTypeTime (time type)
<br>$ CellTypeComboBox (combo box type)
<br>$ CellTypePicture
<br>$ CellTypeCheckBox (checkbox type)
<br>$ CellTypeCurrency
<br>$ CellTypeNumber
<br>$ CellTypePercent
<br>$CellTypeScientific (exponential type)

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the following values. The initial values ​​are $ TypeVAlignCenter for label cells in check box cells, column headers, and row headers, and $ TypeVAlignTop for other cells.
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
    <td class="tg-0lax">$TypeVAlignTop</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Top alignment</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeVAlignBottom</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Bottom alignment</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeVAlignCenter</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Centered</td>
  </tr>
</tbody>
</table>

The horizontal alignment is set with the <a href= "/package/extension5/sspread/properties/typehalign">TypeHAlign</a> property.
The placement of command button cell types is set with the <a href="/package/extension5/sspread/properties/typebuttonalign">TypeButtonAlign</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type ">property inheritance for each data type cell</a> .
<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-combo-box-type-cells">Notes on property inheritance of combo box type cells</a>
<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-label-type-cells">Notes on property inheritance of label type cells</a>

use case
```
Col = 3;
Row = 2;
CellType = $CellTypeStaticText;
TypeHAlign = $TypeHAlignRight;
TypeVAlign = $TypeVAlignBottom;
Text = "sample";
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeNumber;
TypeHAlign = $TypeHAlignLeft;
TypeVAlign = $TypeVAlignCenter;
Value = 12345;
BlockMode = $FALSE;
 ```

Related item

<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typebuttonalign">TypeButtonAlign</a> , <a href= "/package/extension5/sspread/properties/typehalign">TypeHAlign</a> properties