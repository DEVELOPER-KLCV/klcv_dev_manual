---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.MaxTextRowHeight Property
nav_order: 77
permalink: /package/extension5/sspread/properties/maxtextrowheight
---
# {{ page.title }}

Gets the height required to display the text based on the font size set on the line.

This property is an <a href="package/extension5/sspread/#index-property-">Index Property</a>. Specify the row number for the index.

This property is read-only.

Multi-line cells with the <a href="/package/extension5/sspread/properties/typeeditmultiLine">TypeEditMultiLine</a> and <a href="/package/extension5/sspread/properties/typetextwordwrap">TypeTextWordWrap</a>  properties are the height required to display all multi-line text relative to the current column width and font size.

You can display all the text in that row by setting the value of this property to the  <a href="/package/extension5/sspread/properties/rowheight">RowHeight</a> property.

The width of the column can be obtained with the <a href="/package/extension5/sspread/properties/maxtextcolwidth">MaxTextColWidth</a> property.

The  <a href="/package/extension5/sspread/properties/maxtextcellheight">MaxTextCellHeight</a> and <a href="/package/extension5/sspread/properties/maxtextcellwidth">MaxTextCellWidth</a>  properties allow you to get the optimal size for each cell.

Example of usage<br>
```
Row = 2;
Col = 3;
Text = "Biz/Browser";
Col = 4;
Text = "Biz/Designer";
FontSize = 16;
print(MaxTextRowHeight(2), "\n");
RowHeight(2) = MaxTextRowHeight(2);
```

Related Items<br>
<a href="/package/extension5/sspread/properties/maxtextcolwidth">MaxTextColWidth</a>, <a href="/package/extension5/sspread/properties/maxtextcellheight">MaxTextCellHeight</a>,  <a href="/package/extension5/sspread/properties/maxtextcellwidth">MaxTextCellWidth</a>, <a href="/package/extension5/sspread/properties/rowheight">RowHeight</a> property