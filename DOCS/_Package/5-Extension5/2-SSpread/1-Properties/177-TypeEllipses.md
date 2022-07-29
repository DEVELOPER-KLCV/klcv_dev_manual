---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeEllipses Property
nav_order: 177
permalink: /package/extension5/sspread/properties/typeellipses
---
# {{ page.title }}

Set whether to display ellipsis ( ... ) in cells when displaying text that is too long to fit in the cell .

Abbreviated display example<br>
<a href="/img/Package/extension5-sspread-property-typeellipse.jpg" target="_blank">
<img src="/img/Package/extension5-sspread-property-typeellipse.jpg" alt="login image"></a>

Only valid for cells with the following values ​​set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
<br>$CellTypeDate (date type)
<br>$CellTypeEdit (character type)
<br>$CellTypePic (mask type)
<br>$CellTypeStaticText (label type)
<br>$CellTypeTime (time type)
<br>$CellTypeCurrency (currency type)
<br>$CellTypeNumber (numeric type)
<br>$CellTypePercent (percentage type)
<br>$CellTypeScientific (exponential type)

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

This is valid only when the <a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a> property is set to $TypeHAlignLeft (left-aligned) and the <a href="/package/extension5/sspread/properties/typetextorient">TypeTextOrient</a> property is set to $TypeTextOrientHorizontal (horizontal writing).

Also, if the <a href="/package/extension5/sspread/properties/typetextwordwrap">TypeTextWordWrap</a> property of the label type cell and the <a href="/package/extension5/sspread/properties/typeeditmultiline">TypeEditMultiLine</a> property of the character type cell are $TRUE and the display is multi-line, it is invalid.

If the <a href="/package/extension5/sspread/properties/allowcelloverflow">AllowCellOverflow</a> property is set to $ TRUE and the display is overhanging, that will take precedence.

Specify $TRUE to display the ellipsis and $ FALSE to not display it .
<br>The initial value is $FALSE .

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> for each data type cell.
<br><a href="/package/extension5/sspread/properties/celltype#notes-on-property-inheritance-of-label-type-cells">Notes on property inheritance of label type cells</a>

Example of use
```
Col = 3;
Row = 2;
CellType = $CellTypeStaticText;
TypeEllipses = $TRUE;
Text = "Biz / Browser & Biz / Designer";
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeNumber;
TypeHAlign = $TypeHAlignLeft;
TypeEllipses = $TRUE;
Value = 123456789;
BlockMode = $FALSE;
```

Related item<br>
<a href="/package/extension5/sspread/properties/allowcelloverflow">AllowCellOverflow</a> , <a href="/package/extension5/sspread/properties/celltype">CellType</a> , <a href="/package/extension5/sspread/properties/typeeditmultiline">TypeEditMultiLine</a> , <a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a> , <a href="/package/extension5/sspread/properties/typetextorient">TypeTextOrient</a> , <a href="/package/extension5/sspread/properties/typetextwordwrap">TypeTextWordWrap</a> properties
