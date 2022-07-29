---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCurrencyNegStyle Property
nav_order: 162
permalink: /package/extension5/sspread/properties/typecurrencynegstyle
---
# {{ page.title }}

Format a negative number in a currency cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeCurrency(currency type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to process.

Specify the following values. The initial value is $TypeCurrencyNegStyleIntl .
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
    <th class="tg-xt05">Ｃonstant<br></th>
    <th class="tg-2m49">Ｖalue</th>
    <th class="tg-xt05">Ｅxplanation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyleIntl</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Follow OS settings</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle1</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">(\ 1.1)</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle2</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">-\1.1</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle3</td>
    <td class="tg-baqh">3</td>
    <td class="tg-0lax">\-1.1</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle4</td>
    <td class="tg-baqh">4</td>
    <td class="tg-0lax">\ 1.1-</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle5</td>
    <td class="tg-baqh">5</td>
    <td class="tg-0lax">(1.1 \)</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle6</td>
    <td class="tg-baqh">6</td>
    <td class="tg-0lax">-1.1 \</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle7</td>
    <td class="tg-baqh">7</td>
    <td class="tg-0lax">1.1-\</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle8</td>
    <td class="tg-baqh">8</td>
    <td class="tg-0lax">1.1\-</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle9</td>
    <td class="tg-baqh">9</td>
    <td class="tg-0lax">-1.1\</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle10</td>
    <td class="tg-baqh">10</td>
    <td class="tg-0lax">-\ 1.1</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle11</td>
    <td class="tg-baqh">11</td>
    <td class="tg-0lax">1.1 \-</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle12</td>
    <td class="tg-baqh">12</td>
    <td class="tg-0lax">\1.1-</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle13</td>
    <td class="tg-baqh">13</td>
    <td class="tg-0lax">\ -1.1</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle14</td>
    <td class="tg-baqh">14</td>
    <td class="tg-0lax">1.1- \</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle15</td>
    <td class="tg-baqh">15</td>
    <td class="tg-0lax">(\ 1.1)</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeCurrencyNegStyle16</td>
    <td class="tg-baqh">16</td>
    <td class="tg-0lax">(1.1 \)</td>
  </tr>
</tbody>
</table>

You can display negative numbers in red by setting the <a href="/package/extension5/sspread/properties/typenegred">TypeNegRed</a> property to $TRUE .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of currency type cells.

Use case
```
Col = 3;
Row = 2;
CellType = $ CellTypeCurrency;
TypeCurrencyNegStyle = $TypeCurrencyNegStyle1;
Value = -1.23;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeCurrency;
TypeCurrencyNegStyle = $ TypeCurrencyNegStyle3;
Value = -4.56;
BlockMode = $ FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> , 
  <a href="/package/extension5/sspread/properties/typenegred">TypeNegRed</a> property
 