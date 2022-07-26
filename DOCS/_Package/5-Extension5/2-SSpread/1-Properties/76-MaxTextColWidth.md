---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.MaxTextColWidth Property
nav_order: 76
permalink: /package/extension5/sspread/properties/maxtextcolwidth
---
# {{ page.title }}

Get the width required to display the text set in the column.

This property is an <a href="package/extension5/sspread/#index-property-">Index Property</a>. Specify the column number for the index.

This property is read-only.

Finds the column width required to display the text based on the data and font size set for the specified column.
The current column width is used as is for cells displayed in multiple rows by the <a href="/package/extension5/sspread/properties/typeeditmultiLine">TypeEditMultiLine</a> and <a href="/package/extension5/sspread/properties/typetextwordwrap">TypeTextWordWrap</a> property.

You can display all the text in that column by setting the value of this property to the ColWidth property.

The row height can be obtained with the <a href="/package/extension5/sspread/properties/maxtextrowheight">MaxTextRowHeight</a> property.
The <a href="/package/extension5/sspread/properties/maxtextcellheight">MaxTextCellHeight</a> and <a href="/package/extension5/sspread/properties/maxtextcellwidth">MaxTextCellWidth</a> properties allow you to get the optimal size for each cell.

Example of usage<br>
```
Col = 2;
Row = 3;
Text = "Biz/Browser";
Row = 4;
Text = "Biz/Designer";
FontSize = 16;
print(MaxTextColWidth(2), "\n");
ColWidth(2) = MaxTextColWidth(2);
```

Related Items<br>
<a href="/package/extension5/sspread/properties/colwidth">ColWidth</a>, <a href="/package/extension5/sspread/properties/maxtextcellheight">MaxTextCellHeight</a>,  <a href="/package/extension5/sspread/properties/maxtextcellwidth">MaxTextCellWidth</a>, <a href="/package/extension5/sspread/properties/maxtextrowheight">MaxTextRowHeight</a> property