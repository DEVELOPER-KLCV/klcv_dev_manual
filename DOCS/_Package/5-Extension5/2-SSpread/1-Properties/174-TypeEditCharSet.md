---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeEditCharSet Property
nav_order: 174
permalink: /package/extension5/sspread/properties/typeeditcharset
---
# {{ page.title }}

Set the type of characters that can be entered in a cell in a text cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeEdit (character type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the following values. The initial value is $TypeEditCharSetASCII .
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-yj5y{background-color:#efefef;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-y698{background-color:#efefef;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-y698">Constant</th>
    <th class="tg-yj5y">Value</th>
    <th class="tg-y698">Explanation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$TypeEditCharSetASCII</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">All characters</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeEditCharSetAlpha</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">A to Z , a to z , half-width space</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeEditCharSetAlphanumeric</td>
    <td class="tg-c3ow">2</td>
    <td class="tg-0pky">A to Z , a to z , 0 to 9 , half-width space, period ( . ), comma ( , ), minus ( - )</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeEditCharSetNumeric</td>
    <td class="tg-c3ow">3</td>
    <td class="tg-0pky">0 to 9 , period ( . ), minus ( - )</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeEditCharSetKanjiOnly</td>
    <td class="tg-c3ow">4</td>
    <td class="tg-0pky">Full-width characters (*) , half-width spaces</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeEditCharSetKanjiOnlyIME</td>
    <td class="tg-c3ow">5</td>
    <td class="tg-0pky">Full- width characters (*) , half-width spaces ( IME automatic ON / OFF )</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeEditCharSetAllIME</td>
    <td class="tg-c3ow">6</td>
    <td class="tg-0pky">All characters ( IME auto ON/OFF )</td>
  </tr>
</tbody>
</table>
*Full-width characters: Characters other than half-width alphanumeric characters, half-width symbols, and half-width kana

It applies to all input data, including user input, pasting from the clipboard, and setting values ​​from scripts.
<br>It does not apply to the data already set in the cell when you change this property.

$TypeEditCharSetKanjiOnlyIME and $TypeEditCharSetAllIME control IME. IME is automatically turned on when the target cell becomes the active cell . IME is automatically turned off when the target cell is no longer the active cell.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for character cells.

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypeEdit;
TypeEditCharSet = $TypeEditCharSetAlpha;
Text = "sample";
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeEdit;
TypeEditCharSet = $TypeEditCharSetAllIME;
Text = " Ah ";
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a>  property