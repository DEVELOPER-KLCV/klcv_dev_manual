---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeDateFormat Property
nav_order: 169
permalink: /package/extension5/sspread/properties/typedateformat
---
# {{ page.title }}

Set the date display format in a date type cell.

Valid only for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeDate (date type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to do.

Specify the following values. The initial value is the setting value of the OS.
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-8r26{background-color:#D9D9D9;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant</th>
    <th class="tg-8r26">Value</th>
    <th class="tg-kg9c">Example ( 2011年5月24日 )</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$TypeDateFormatDDMONYY</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">24 / May / 2011</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeDateFormatDDMMYY</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">24/05/2011</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeDateFormatMMDDYY</td>
    <td class="tg-c3ow">2</td>
    <td class="tg-0pky">05/24/2011</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeDateFormatYYMMDD</td>
    <td class="tg-c3ow">3</td>
    <td class="tg-0pky">2011/05/24</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeDateFormatYYMM</td>
    <td class="tg-c3ow">4</td>
    <td class="tg-0pky">2011/05</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeDateFormatMMDD</td>
    <td class="tg-c3ow">5</td>
    <td class="tg-0pky">05/24</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeDateFormatGEEMMDD</td>
    <td class="tg-c3ow">6</td>
    <td class="tg-0pky">H23/05/24</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeDateFormatGGEEMMDD</td>
    <td class="tg-c3ow">7</td>
    <td class="tg-0pky">平23/05/24</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeDateFormatGGGGEEMMDD</td>
    <td class="tg-c3ow">8</td>
    <td class="tg-0pky">平成2011/05/24</td>
  </tr>
  <tr>
    <td class="tg-0pky">$TypeDateFormatDefault</td>
    <td class="tg-c3ow">99</td>
    <td class="tg-0pky">Returns to the initial value. (For setting only)</td>
  </tr>
</tbody>
</table>

The number of digits in the Christian era ( 2 digits, 4 digits) is set by the <a href="/package/extension5/sspread/properties/typedatecentury">TypeDateCentury</a> property.
<br>The year / month / day delimiter is set with the <a href="/package/extension5/sspread/properties/typedateseparator">TypeDateSeparator</a> property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for date cells.

Example of use
```
Col = 3;
Row = 2;
CellType = $CellTypeDate;
TypeDateFormat = $ TypeDateFormatGGGGEEMMDD;
Value = str(sysdate(), "YYYYMMDD");
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeDate;
TypeDateFormat = $TypeDateFormatDDMONYY;
Value = str(sysdate(), "YYYYMMDD");
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typedatecentury">TypeDateCentury</a> , <a href="/package/extension5/sspread/properties/typedateseparator">TypeDateSeparator</a>  properties