---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeNumberNegStyle Property
nav_order: 186
permalink: /package/extension5/sspread/properties/typenumbernegstyle
---
# {{ page.title }}

Formats negative numbers in numeric cells.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeNumber (numeric type).
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.


Specify the following values. The initial value is $TypeNumberNegStyleIntl .

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
    <td class="tg-0lax">$ TypeNumberNegStyleIntl</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Follow OS settings</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeNumberNegStyle1</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">(1.1)</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeNumberNegStyle2</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">-1.1</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeNumberNegStyle3</td>
    <td class="tg-baqh">3</td>
    <td class="tg-0lax">--1.1 1.1</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeNumberNegStyle4</td>
    <td class="tg-baqh">4</td>
    <td class="tg-0lax">1.1-</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeNumberNegStyle5</td>
    <td class="tg-baqh">5</td>
    <td class="tg-0lax">1.1 -</td>
  </tr>
</tbody>
</table>

Negative numbers can be displayed in red by setting the <a href="/package/extension5/sspread/properties/typenegred">TypeNegRed</a> property to $TRUE.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for numeric cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeNumber;
TypeNumberNegStyle = $ TypeNumberNegStyle1;
Value = -1.23;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeNumber;
TypeNumberNegStyle = $ TypeNumberNegStyle3;
Value = -4.56;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typenegred">TypeNegRed</a> property