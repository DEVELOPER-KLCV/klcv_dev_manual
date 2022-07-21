---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ColWidth Property
nav_order: 40
permalink: /package/extension5/sspread/properties/colwidth
---
# {{ page.title }}

Sets the width of the column.

This property is an <a href="package/extension5/sspread/#index-property-">Index Property</a>. Specify the following values for the index.

| Index           | Description                      |
|-----------------|----------------------------------|
| 0               | Line header                      |
| -1              | All columns                      |
| -2              | Column specified by Col property |
| Other than that | Column index                     |

The initial value is 64 .

The row height is set with the <a href="/package/extension5/sspread/properties/rowheight">RowHeight</a> property.

To allow the user to change the width of the column, set the <a href="/package/extension5/sspread/properties/userresize">UserResize</a> and <a href="/package/extension5/sspread/properties/userresizecol">UserResizeCol</a> properties.

The <a href="/package/extension5/sspread/events/colwidthchange">ColWidthChange</a> event is fired when the user changes the width of a column .

The <a href="/package/extension5/sspread/properties/maxtextcellwidth">MaxTextCellWidth</a> and <a href="/package/extension5/sspread/properties/maxtextcolwidth">MaxTextColWidth</a> properties can be used to get the required width based on the data set in the cell.

Example of usage <br>
```
ColWidth(-1) = 100;
ColWidth(2) = 200;
 
Col = 3;
ColWidth(-2) = 300;
 
print(ColWidth(1), ColWidth(2), ColWidth(3), "\n");
```

Related Items<br>
<a href="/package/extension5/sspread/properties/maxtextcellwidth">MaxTextCellWidth</a>, <a href="/package/extension5/sspread/properties/maxtextcolwidth">MaxTextColWidth</a>, <a href="/package/extension5/sspread/properties/rowheight">RowHeight</a>, <a href="/package/extension5/sspread/properties/userresize">UserResize</a>, <a href="/package/extension5/sspread/properties/userresizecol">UserResizeCol</a> property <br>
<a href="/package/extension5/sspread/events/colwidthchange">ColWidthChange</a> event