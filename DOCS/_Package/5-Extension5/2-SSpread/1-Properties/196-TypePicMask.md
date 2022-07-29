---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypePicMask Property
nav_order: 196
permalink: /package/extension5/sspread/properties/typepicmask
---
# {{ page.title }}

Format the mask input in the mask cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypePicture.
<br>Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The character types that can be entered and their digit positions are set using the following definition characters. Only the character type corresponding to the definition character can be entered at the position where the definition character is set.

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
<table class="tg" style="undefined;table-layout: fixed; width: 717px">
<colgroup>
<col style="width: 136.005682px">
<col style="width: 581.005682px">
</colgroup>
<thead>
  <tr>
    <th class="tg-2m49">Definition character</th>
    <th class="tg-xt05">Character types that can be input</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-baqh">X</td>
    <td class="tg-0lax">All characters (half-width and full-width)</td>
  </tr>
  <tr>
    <td class="tg-baqh">9</td>
    <td class="tg-0lax">Half-width numbers and decimal points</td>
  </tr>
  <tr>
    <td class="tg-baqh">A</td>
    <td class="tg-0lax">Half-width alphabet characters</td>
  </tr>
  <tr>
    <td class="tg-baqh">N</td>
    <td class="tg-0lax">Half-width alphabetic characters, half-width numbers and decimal point</td>
  </tr>
  <tr>
    <td class="tg-baqh">U</td>
    <td class="tg-0lax">Half-width uppercase letters</td>
  </tr>
  <tr>
    <td class="tg-baqh">L</td>
    <td class="tg-0lax">Half-width lowercase letters</td>
  </tr>
  <tr>
    <td class="tg-baqh">H</td>
    <td class="tg-0lax">Half - width hexadecimal numbers ( 0-9 , a - f , A - F )</td>
  </tr>
  <tr>
    <td class="tg-baqh">&amp;</td>
    <td class="tg-0lax">Full- width characters (*) , half-width spaces<br>* Characters other than half-width alphanumericals, half-width symbols, and half-width kana</td>
  </tr>
</tbody>
</table>

If you specify a character other than the above, that character is fixedly displayed and the input to that digit position is skipped.
If you want to pin the above definition characters themselves, you can escape them with a / (slash) in front of them ( / A , / X , / & , etc.).
If you overlap the slashes ( // ), the slashes themselves will be fixed.

The initial value is a blank character string.

The <a href="/package/extension5/sspread/properties/TypePercentNegStyleIntl">TypePicDefaultText</a> property allows you to set the character to be displayed as the initial value at the position of the definition character.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for masked cells .

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypePic;
TypePicMask = "999-9999";
TypePicDefaultText = "000-0000";
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypePic;
TypePicMask = "U99.99.99～U99.99.99";
TypePicDefaultText = "#__.__.__～#__.__.__";
BlockMode = $FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/TypePercentNegStyleIntl">TypePicDefaultText</a> properties.