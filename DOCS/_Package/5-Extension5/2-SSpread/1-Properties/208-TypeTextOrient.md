---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeTextOrient Property
nav_order: 208
permalink: /package/extension5/sspread/properties/typetextorient
---
# {{ page.title }}
Set the display direction of the text in the cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a>  property.
<br>$CellTypeDate(date type)
<br>$CellTypeEdit(character type)
<br>$CellTypePic(mask type)
<br>$CellTypeStaticText(label type)
<br>$CellTypeTime
<br>$CellTypeCurrency
<br>$CellTypeNumber
<br>$CellTypePercent
<br>$CellTypeScientific


Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the following values. The initial value is $ TypeTextOrientHorizontal.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-8r26{background-color:#D9D9D9;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant</th>
    <th class="tg-8r26">Value</th>
    <th class="tg-kg9c">Explanation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$TypeTextOrientHorizontal</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">Horizontal writing</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeTextOrientVerticalLTR</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">Vertical writing (folding from left to right)</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeTextOrientDown</td>
    <td class="tg-c3ow">2</td>
    <td class="tg-0pky">90 degree rotation (downward)</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeTextOrientUp</td>
    <td class="tg-c3ow">3</td>
    <td class="tg-0pky">270 degree rotation (upward)</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeTextOrientInvert</td>
    <td class="tg-baqh">4</td>
    <td class="tg-0lax">180 degree rotation (reversal)</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeTextOrientVerticalRTL</td>
    <td class="tg-baqh">5</td>
    <td class="tg-0lax">Vertical writing (folding from right to left)</td>
  </tr>
</tbody>
</table>
 

If the input mode ( <a href="/package/extension5/sspread/properties/editmode">EditMode</a> property is $TRUE ), the display is normal (horizontal writing, no rotation).

The wrapping direction of $TypeTextOrientVerticalLTR and $TypeTextOrientVerticalRTL (vertical writing) is the direction for multi-line display (<a href= "/package/extension5/sspread/properties/typetextwordwrap">TypeTextWordWrap</a> for label type cells , <a href= "/package/extension5/sspread/properties/typeeditmultiline">TypeEditMultiLine</a> property for character type cells is $TRUE ).

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for each data type cells .
<a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">Notes on property inheritance of each data type cells.</a>

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeEdit;
TypeTextOrient = $ TypeTextOrientInvert;
Value = "sample";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeNumber;
TypeTextOrient = $ TypeTextOrientDown;
Value = 10;
BlockMode = $ FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>  property