---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeEditCharCase Property
nav_order: 173
permalink: /package/extension5/sspread/properties/typeeditcharcase
---
# {{ page.title }}

Set whether text cells are automatically converted to uppercase or lowercase.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeEdit (text type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to process.

Specify the following values. The initial value is $TypeEditCharCaseSetNone.
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
    <td class="tg-0lax">$ TypeEditCharCaseSetLower</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Convert to lowercase</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeEditCharCaseSetNone</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">No conversion</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeEditCharCaseSetUpper</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Convert to uppercase</td>
  </tr>
</tbody>
</table>

It applies to all input data, including user input, pasting from the clipboard, and setting values ​​from scripts.
<br>It does not apply to the data already set in the cell when you change this property.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for character cells.

Use case
```
Col = 3;
Row = 2;
CellType = $ CellTypeEdit;
TypeEditCharCase = $ TypeEditCharCaseSetLower;
Text = "abcDEF";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeEdit;
TypeEditCharCase = $ TypeEditCharCaseSetUpper;
Text = "abcDEF";
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a>  property