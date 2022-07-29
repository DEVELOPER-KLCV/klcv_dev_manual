---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.MaxTextCellHeight Property
nav_order: 74
permalink: /package/extension5/sspread/properties/maxtextcellheight
---
# {{ page.title }}

Gets the height required to display the text set in the cell.

Before referencing this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties to specify the target cell.

This property is read-only. 

Find the height required to display the text based on the font size set in the cell.

Multi-line cells with the <a href="/package/extension5/sspread/properties/typeeditmultiLine">TypeEditMultiLine</a> and <a href="/package/extension5/sspread/properties/typetextwordwrap">TypeTextWordWrap</a> properties return the height required to display all multi-line text relative to the current column width and font size.

By using the <a href="/package/extension5/sspread/properties/maxtextcellwidth">MaxTextCellWidth</a> and MaxTextCellHeight properties, you can find the optimum size according to the state of the cell.

The <a href="/package/extension5/sspread/properties/maxtextrowheight">MaxTextRowHeight</a> property allows to get the required height of the entire row.

Example of usage<br>
```
Col = 2;
Row = 3;
Text = "Biz/Browser";
print(MaxTextCellWidth , MaxTextCellHeight, "\n");
ColWidth(2) = MaxTextCellWidth;
RowHeight(3) = MaxTextCellHeight;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/maxtextcellwidth">MaxTextCellWidth</a>, <a href="/package/extension5/sspread/properties/maxtextrowheight">MaxTextRowHeight</a>, <a href="/package/extension5/sspread/properties/rowheight">RowHeight</a> property