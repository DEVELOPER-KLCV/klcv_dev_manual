---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypePercentNegStyle Property
nav_order: 194
permalink: /package/extension5/sspread/properties/typepercentnegstyle
---
# {{ page.title }}

Formats negative numbers in percentage cells.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypePicture.
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the following values. The initial value is $TypePercentNegStyleIntl.

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
    <td class="tg-0lax">$ TypePercentNegStyleIntl</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Follow OS settings</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypePercentNegStyle1</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">(1.1%)</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypePercentNegStyle2</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">-1.1%</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypePercentNegStyle3</td>
    <td class="tg-baqh">3</td>
    <td class="tg-0lax">1.1 – %</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypePercentNegStyle4</td>
    <td class="tg-baqh">4</td>
    <td class="tg-0lax">1.1%-</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypePercentNegStyle5</td>
    <td class="tg-baqh">5</td>
    <td class="tg-0lax">-1.1%</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypePercentNegStyle6</td>
    <td class="tg-baqh">6</td>
    <td class="tg-0lax">1.1%-</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypePercentNegStyle7</td>
    <td class="tg-baqh">7</td>
    <td class="tg-0lax">1.1 – %</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypePercentNegStyle8</td>
    <td class="tg-baqh">8</td>
    <td class="tg-0lax">(1.1%)</td>
  </tr>
</tbody>
</table>

Negative numbers can be displayed in red by setting the <a href="/package/extension5/sspread/properties/typenegred">TypeNegRed</a> property to $TRUE.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for percentage cells .

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypePercent;
TypePercentNegStyle = $ TypePercentNegStyle1;
Value = -0.123;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypePercent;
TypePercentNegStyle = $ TypePercentNegStyle3;
Value = -0.456;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typenegred">TypeNegRed</a> properties.