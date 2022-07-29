---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeCurrencyMin Property
nav_order: 161
permalink: /package/extension5/sspread/properties/typecurrencymin
---
# {{ page.title }}

Set the maximum value that can be entered in a currency type cell.

Only valid for cells with the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property set to $CellTypeCurrency(currency type).
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> , <a href="/package/extension5/sspread/properties/row">Row</a> properties etc. to specify what you want to process.

The initial value is -9999999.99 .

The upper limit is specified by the <a href="/package/extension5/sspread/properties/typecurrencymax">TypeCurrencyMax</a> property.
The spin button displayed by the <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a> property allows you to increase or decrease the value within the specified range. When the <a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a> property is set to $TRUE , the values ​​that have reached the upper and lower limits are wrapped.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">property inheritance</a> of currency type cells.

<a href="/package/extension5/sspread/#precautions-for-specifying-the-range-based-on-the-lower-and-upper-limits-">Precautions for specifying the range based on the lower and upper limits</a>

Use case
```
Col = 3;
Row = 2;
CellType = $CellTypeCurrency;
TypeCurrencyMin = 0;
TypeCurrencyMax = 100;
Value = 0;
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeCurrency;
TypeCurrencyMin = -100;
TypeCurrencyMax = 100;
Value = 0;
BlockMode = $FALSE;
```

Related item<br>
 <a href="/package/extension5/sspread/properties/celltype">CellType</a> , 
  <a href="/package/extension5/sspread/properties/typecurrencymax">TypeCurrencyMax</a> ,  <a href="/package/extension5/sspread/properties/typespin">TypeSpin</a> ,  <a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a> property
 