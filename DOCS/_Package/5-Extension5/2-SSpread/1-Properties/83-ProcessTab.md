---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ProcessTab Property
nav_order: 83
permalink: /package/extension5/sspread/properties/processtab
---
# {{ page.title }}

Set whether to move the active cell with the Tab key.

Specify $TRUE to move the active cell and $FALSE to move the focus to another object.

The initial value is $FALSE.

Normally, the Tab key is used to move the focus between objects, but setting this property to $TRUE allows you to use the Tab key to move the active cell in the spreadsheet.

If you use the Tab key to move the active cell, pressing the Tab key moves the active cell to the next cell (the cell on the right, or the first cell in the next row if it is the last column). Press Shift + Tab to move the active cell to the previous cell (the left cell, or the last column of the previous row in the case of the first column).

Related Items<br>
<a href="/package/extension5/sspread/properties/arrowsexiteditmode">ArrowsExitEditMode</a>, <a href="/package/extension5/sspread/properties/editenteraction">EditEnterAction</a> properties