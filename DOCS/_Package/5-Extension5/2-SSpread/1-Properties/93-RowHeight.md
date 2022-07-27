---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.RowHeight Property
nav_order: 93
permalink: /package/extension5/sspread/properties/rowheight
---
# {{ page.title }}

Set the row height.

This property is an <a href="package/extension5/sspread/#index-property-">Index Property</a>. Specify the following values for the index.

| Index | Description                   |
|:-----:|-------------------------------|
|   0   | Column header                 |
|   -1  | All rows                      |
|   -2  | Row specified by Row property |
| Other | Row number                    |

The initial value is 15.

The width of the column is set with the <a href="/package/extension5/sspread/properties/colwidth">ColWidth</a> property.

To allow the user to change the row height, set the <a href="/package/extension5/sspread/properties/userresize">UserResize</a> and <a href="/package/extension5/sspread/properties/userresizerow">UserResizeRow</a> properties.
The <a href="/package/extension5/sspread/events/rowheightchange">RowHeightChange</a> event is raised when the user changes the row height.

You can use the <a href="/package/extension5/sspread/properties/maxtextcellheight">MaxTextCellheight</a> and <a href="/package/extension5/sspread/properties/maxtextrowheight">MaxTextRowheight</a> properties to get the required height based on the data set in the cell.

Example of usage<br>
```
RowHeight(-1) = 20;
RowHeight(2) = 40;
 
Row = 3;
RowHeight(-2) = 60;
 
print(RowHeight(1), RowHeight(2), RowHeight(3), "\n");
```

Related Items<br>
<a href="/package/extension5/sspread/properties/maxtextcellheight">MaxTextCellheight</a>, <a href="/package/extension5/sspread/properties/maxtextrowheight">MaxTextRowheight</a>, <a href="/package/extension5/sspread/properties/colwidth">ColWidth</a>, <a href="/package/extension5/sspread/properties/userresize">UserResize</a>, <a href="/package/extension5/sspread/properties/userresizerow">UserResizeRow</a>  property<br>
<a href="/package/extension5/sspread/events/rowheightchange">RowHeightChange</a> event