---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.Clip Property
nav_order: 28
permalink: /package/extension5/sspread/properties/clip
---
# {{ page.title }}

Set the value in the cell block.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

(This property does not require the <a href="/package/extension5/sspread/properties/blockmode">BlockMode</a> property to be set to $TRUE in advance when dealing with cell blocks.)

The value for each cell is set by separating the columns with the tab character (￥ t) and the rows with the newline character (￥ r ￥ n).

Clip behaves as if you were setting a value in the <a href="/package/extension5/sspread/properties/text">Text</a> property for each cell. It is more efficient than setting it for individual cells with the Text property.

<a href="package/extension5/sspread/#get-and-set-the-value-for-each-cell-data-type-">Get and set the value for each cell data type</a> 

Example of usage<br>
```
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
Clip = "あ￥tい￥tう￥r￥nア￥tイ￥tウ￥r￥nＡ￥tＢ￥tＣ";
 
Col = 4;
Row = 4;
Col2 = 5;
Row2 = 5;
print(Clip);
```

Related Items <br>
<a href="/package/extension5/sspread/properties/clipvalue">ClipValue</a>, <a href="/package/extension5/sspread/properties/text">Text</a> property
