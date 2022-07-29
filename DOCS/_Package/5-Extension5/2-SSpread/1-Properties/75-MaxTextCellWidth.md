---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.MaxTextCellWidth Property
nav_order: 75
permalink: /package/extension5/sspread/properties/maxtextcellwidth
---
# {{ page.title }}

Gets the width required to display the text set in the cell.

Before referencing this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties to specify the target cell.

This property is read-only.
Find the width required to display the text based on the data and font size set in the cell.

For multi-row cells with the <a href="/package/extension5/sspread/properties/typeeditmultiLine">TypeEditMultiLine</a> and <a href="/package/extension5/sspread/properties/typetextwordwrap">TypeTextWordWrap</a> properties, the current column width is returned as is.

By using the MaxTextCellWidth and <a href="/package/extension5/sspread/properties/maxtextcellheight">MaxTextCellHeight</a> properties, you can find the optimum size according to the state of the cell.

The <a href="/package/extension5/sspread/properties/maxtextcolwidth">MaxTextColWidth</a> property can get the required width for the entire column.

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
<a href="/package/extension5/sspread/properties/maxtextcellheight">MaxTextCellHeight</a>, <a href="/package/extension5/sspread/properties/maxtextcolwidth">MaxTextColWidth</a>, <a href="/package/extension5/sspread/properties/colwidth">ColWidth</a> property