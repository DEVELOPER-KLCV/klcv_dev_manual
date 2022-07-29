---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.Text Property
nav_order: 128
permalink: /package/extension5/sspread/properties/text
---
# {{ page.title }}

Set values such as strings, numbers, and dates in cells.

Before setting this property, use the 
Changing this property does not affect the <a href="/package/extension5/sspread/properties/col">Col</a>, 
Changing this property does not affect the <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

The initial value is a blank character string.

This property has different acquisition and setting rules depending on the cell data type (<a href="/package/extension5/sspread/properties/celltype">CellType</a> property).
For details, refer to <a href="package/extension5/sspread/#get-and-set-the-value-for-each-cell-data-type->Get and set the value for each cell data type</a> 
<a href="package/extension5/sspread/#index-property-">Index Property</a>.

The string can be obtained before formatting with the <a href="/package/extension5/sspread/properties/value">Value</a> property and the formatted string with the Text property.

Example of usage<br>
```
Col = 2;
Row = 3;
Text = "sample1";
 
BlockMode = $TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
Text ="sample2";
BlockMode = $FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/clip">Clip</a>, <a href="/package/extension5/sspread/properties/value">Value</a>  property<br>
<a href="/package/extension5/sspread/methods/gettext">GetText</a>, <a href="/package/extension5/sspread/methods/settext">SetText</a> method
