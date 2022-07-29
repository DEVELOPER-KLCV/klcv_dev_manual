---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeNumberLeadingZero Property
nav_order: 183
permalink: /package/extension5/sspread/properties/typenumberleadingzero
---
# {{ page.title }}

Sets whether to display leading zeros in numeric cells.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeNumber (numeric type).
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the following values. The initial value is $ TypeLeadingZeroIntl .

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
    <td class="tg-0lax">$ TypeLeadingZeroIntl</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Follow OS settings</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeLeadingZeroNo</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Hide</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeLeadingZeroYes</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Display</td>
  </tr>
</tbody>
</table>

This property specifies whether to display zeros in the integer part for decimal values ​​between -1.0 and 1.0 .

For example , at -0.5 , it will be " -0.5 " if it is displayed, and " -.5 " if it is not displayed .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for numeric cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeNumber;
TypeNumberLeadingZero = $ TypeLeadingZeroNo;
Value = 0.23;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeNumber;
TypeNumberLeadingZero = $ TypeLeadingZeroYes;
Value = 0.45;
BlockMode = $ FALSE;
 
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>  property