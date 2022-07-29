---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.TypeButtonAlign Property
nav_order: 133
permalink: /package/extension5/sspread/properties/typebuttonalign
---
# {{ page.title }}

In the command button type cell, set where to place the text with respect to the set image.

Only valid for cells with $CellTypeButton (command button type) set in the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property.
Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the following values. The initial value is $TypeButtonAlignBottom.

| Constant               | Value | Description                         |
|------------------------|:-----:|-------------------------------------|
| $TypeButtonAlignBottom |   0   | Place text below image              |
| $TypeButtonAlignTop    |   1   | Place text on top of the image      |
| $TypeButtonAlignLeft   |   2   | Place text to the left of the image |
| $TypeButtonAlignRight  |   3   | Place text to right of image        |

The text displayed on the command button is set with the <a href="/package/extension5/sspread/properties/typebuttontext">TypeButtonText</a> property.
If the image is not set in the <a href="/package/extension5/sspread/properties/typebuttonpicture">TypeButtonPicture</a> property and <a href="/package/extension5/sspread/properties/typebuttonpicturedown">TypeButtonPictureDown</a> property, the text will be displayed in the center.

This property is subject to <a href="/package/extension5/sspread/properties/celltype#property-inheritance-for-each-cell-data-type">Property inheritance </a> for command button cells.

Example of usage<br>
```
Col = 3;
Row = 2;
CellType = $CellTypeButton;
TypeButtonText = " Button 1";
TypeButtonPicture = "sample1.png";
TypeButtonAlign = $ TypeButtonAlignTop;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $CellTypeButton;
TypeButtonText = " Button 2";
TypeButtonPicture = "sample2.png";
TypeButtonAlign = $ TypeButtonAlignLeft;
BlockMode = $ FALSE;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/typebuttonpicture">TypeButtonPicture</a>, <a href="/package/extension5/sspread/properties/typebuttonpicturedown">TypeButtonPictureDown</a>, <a href="/package/extension5/sspread/properties/typebuttontext">TypeButtonText</a>  properties