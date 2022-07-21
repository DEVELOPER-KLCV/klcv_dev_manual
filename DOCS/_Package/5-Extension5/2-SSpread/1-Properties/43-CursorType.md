---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.CursorType Property
nav_order: 43
permalink: /package/extension5/sspread/properties/cursortype
---
# {{ page.title }}

Sets the area to be changed when changing the mouse cursor. Different mouse cursors  can be set for specific areas and states of your spreadsheet.

Specify the following values. The initial value is $CursorTypeDefault.

| Constant                | Value | Description                                                                                                          |
|-------------------------|:-----:|----------------------------------------------------------------------------------------------------------------------|
| $CursorTypeDefault      |   0   | Spreadsheet cell                                                                                                     |
| $CursorTypeColResize    |   1   | Position to change the width of the column (between the column headers)                                              |
| $CursorTypeRowResize    |   2   | Position to change line height (between line headers)                                                                |
| $CursorTypeButton       |   3   | Command button (<a href="/package/extension5/sspread/properties/celltype">CellType</a> property is $CellTypeButton ) |
| $CursorTypeGrayArea     |   4   | Gray area (to the right of the last column, below the last row)                                                      |
| $CursorTypeLockedCell   |   5   | Locked cell                                                                                                          |
| $CursorTypeColHeader    |   6   | Column header                                                                                                        |
| $CursorTypeRowHeader    |   7   | Line header                                                                                                          |
| $CursorTypeDragDropArea |   8   | Start position of drag and drop of cell block                                                                        |
| $CursorTypeDragDrop     |   9   | While dragging a cell block                                                                                          |

The mouse cursor does not change when this property is set. When you set a value for the <a href="/package/extension5/sspread/properties/cursorstyle">CursorStyle</a> property, the target mouse cursor set for this property is changed.

Example of usage<br>
```
CursorType = $CursorTypeDefault;
CursorStyle = $CursorStyleArrow;
 
CursorIcon = "lock.ani";
CursorType = $CursorTypeLockedCell;
CursorStyle = $CursorStyleUserDefined;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/cursoricon">CursorIcon</a>, <a href="/package/extension5/sspread/properties/cursorstyle">CursorStyle</a>, <a href="/package/extension5/sspread/properties/userresize">UserResize</a><a href="/package/extension5/sspread/properties/celltype">CellType</a><a href="/package/extension5/sspread/properties/lock">Lock</a>, <a href="/package/extension5/sspread/properties/allowdragdrop">AllowDragDrop</a> property