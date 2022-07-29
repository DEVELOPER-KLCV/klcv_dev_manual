---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeComboBoxAutoSearch Property
nav_order: 148
permalink: /package/extension5/sspread/properties/typecomboboxautosearch
---
# {{ page.title }}

Set the search type when searching for list items by character input in a combo box type cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeComboBox (combo box type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to process.

Specify the following values. The initial value is $TypeComboBoxAutoSearchSingleChar .
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
    <td class="tg-0lax">$TypeComboBoxAutoSearchNone</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Not specified</td>
  </tr>
  <tr>
    <td class="tg-0lax">$TypeComboBoxAutoSearchSingleChar</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">specify 1 character<br>The list item of "1 entered character = the first character of the list item" is selected.<br>If there is no matching item in the list, it will not be selected.</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeComboBoxAutoSearchMultipleChar</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Specify multiple characters<br>A list item that matches with frontwards multiple characters input will be selected.<br>If there is no matching item in the list, it will not be selected.</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ TypeComboBoxAutoSearchSingleCharGreater</td>
    <td class="tg-baqh">3</td>
    <td class="tg-0lax">Specify one character (search for subsequent characters as well)<br>The list item of "1 entered character = the first character of the list item" is selected.<br>If there is no match in the list, search for the next character ( b for a ).</td>
  </tr>
</tbody>
</table>
Setting this property to something other than $TypeComboBoxAutoSearchNone allows the user to select a combo box list item by typing on the keyboard.

This feature is enabled only if the <a href="/package/extension5/sspread/properties/typecomboboxeditable">TypeComboBoxEditable</a> property is $FALSE .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of combo box type cells.
<a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-combo-box-type-cells">Notes on property inheritance of combo box type cells</a>

### Example of searching buy character input

list item
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">aaa</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">abc</td>
  </tr>
  <tr>
    <td class="tg-0lax">bbb</td>
  </tr>
  <tr>
    <td class="tg-0lax">bcd</td>
  </tr>
  <tr>
    <td class="tg-0lax">xyz</td>
  </tr>
</tbody>
</table>

 $TypeComboBoxAutoSearchSingleChar - single character
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05">Key to enter</th>
    <th class="tg-xt05">Selected item</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">a</td>
    <td class="tg-0lax">aaa</td>
  </tr>
  <tr>
    <td class="tg-0lax">b</td>
    <td class="tg-0lax">bbb</td>
  </tr>
  <tr>
    <td class="tg-0lax">c</td>
    <td class="tg-0lax">not selected</td>
  </tr>
  <tr>
    <td class="tg-0lax">a → a</td>
    <td class="tg-0lax">aaa → abc</td>
  </tr>
  <tr>
    <td class="tg-0lax">a → b</td>
    <td class="tg-0lax">aaa → bbb</td>
  </tr>
</tbody>
</table>

 $TypeComboBoxAutoSearchMultipleChar - specify multiple characters
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05">Key to enter</th>
    <th class="tg-xt05">Selected item</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">a</td>
    <td class="tg-0lax">aaa</td>
  </tr>
  <tr>
    <td class="tg-0lax">b</td>
    <td class="tg-0lax">bbb</td>
  </tr>
  <tr>
    <td class="tg-0lax">c</td>
    <td class="tg-0lax">not selected</td>
  </tr>
  <tr>
    <td class="tg-0lax">a → a</td>
    <td class="tg-0lax">aaa</td>
  </tr>
  <tr>
    <td class="tg-0lax">a → b</td>
    <td class="tg-0lax">aaa → abc</td>
  </tr>
</tbody>
</table>

 $TypeComboBoxAutoSearchSingleCharGreater - specify one character (also search for subsequent characters)
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05">Key to enter</th>
    <th class="tg-xt05">Selected item</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">a</td>
    <td class="tg-0lax">aaa</td>
  </tr>
  <tr>
    <td class="tg-0lax">b</td>
    <td class="tg-0lax">bbb</td>
  </tr>
  <tr>
    <td class="tg-0lax">c</td>
    <td class="tg-0lax">xyz</td>
  </tr>
  <tr>
    <td class="tg-0lax">a → a</td>
    <td class="tg-0lax">aaa → abc</td>
  </tr>
  <tr>
    <td class="tg-0lax">a → b</td>
    <td class="tg-0lax">aaa → bbb</td>
  </tr>
</tbody>
</table>
This is an example of operation from the unselected state. When an item is selected, search after it.

Example of use
```
Col = 3;
Row = 2;
CellType = $ CellTypeComboBox;
TypeComboBoxAutoSearch = $ TypeComboBoxAutoSearchSingleChar;
TypeComboBoxList = "aaa \ tabc \ tbbb \ tbcd \ txyz";
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeComboBox;
TypeComboBoxAutoSearch = $TypeComboBoxAutoSearchMultipleChar;
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typecomboboxeditable">TypeComboBoxEditable </a>  property