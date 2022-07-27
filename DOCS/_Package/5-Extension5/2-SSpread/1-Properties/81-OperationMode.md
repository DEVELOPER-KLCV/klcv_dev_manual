---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.OperationMode Property
nav_order: 81
permalink: /package/extension5/sspread/properties/operationmode
---
# {{ page.title }}

Sets the spreadsheet operating mode.

Specify the following values. The initial value is $OperationModeNormal.

| Constant               | Value | Description                | Data editing |
|------------------------|:-----:|----------------------------|:------------:|
| $OperationModeNormal   |   0   | Normal mode              |      Yes     |
| $OperationModeRead     |   1   | Read-only mode             |      No      |
| $OperationModeRow      |   2   | Row mode                   |      Yes     |
| $OperationModeSingle   |   3   | Single selection mode      |      No      |
| $OperationModeMulti    |   4   | Multiple selection mode    |      No      |
| $OperationModeExtended |   5   | Extended multi-select mode |      No      |

※ Changing this property will significantly change the behavior of the spreadsheet and will have a significant impact on other properties and methods, so as a general rule, set it first when initializing the SSpread object. We do not recommend programs that switch over and over while working with spreadsheets.

### Normal Mode ($OperationModeNormal)
 
It works like spreadsheet software. It is used when entering and displaying data on a cell-by-cell basis.

Clicking on a row selects that one row, and clicking on a column selects that one column.

Clicking on a cell will move the focus to that cell. Double-click the cell to enter input mode.

### Read-only Mode ($OperationModeRead)
 
Operates as a tabular display control.

The user cannot edit the cell. Clicking on a cell does not display a focus frame that indicates the active cell.

### Row Mode ($OperationModeRow)
 
Use this when you want to enter data line by line. This is convenient when you want to enter detailed data one by one.

There are two states in row mode. Normally, it operates like "single selection mode" and data cannot be edited. If you double-click a cell, it will be in the row edit state, and only that row will operate like "standard mode" and you will be able to edit the data. Click other than that line to finish editing.

The <a href="/package/extension5/sspread/events/enterrow">EnterRow</a> event is fired when the row edit state is reached, and the <a href="/package/extension5/sspread/events/leaverow">LeaveRow</a> event is fired when the row edit state is finished.

### Single Selection Mode ($OperationModeSingle)
 
Operates as a list-type display control (single selection). It is used for single selection of detailed data.
The user cannot edit the cell. Focus does not move to individual cells.
Click a cell to select that row. Multiple lines cannot be selected.
Get the selected line number with the <a href="/package/extension5/sspread/properties/selmodeindex">SelModeIndex</a> property.


### Multiple Selection Mode ($OperationModeMulti)

Operates as a list-type display control (multiple selection). It is used when you want to select multiple item data at the same time.

The user cannot edit the cell. Focus does not move to individual cells.
Click a cell to select that row. Multiple additional rows can be selected.
Click the selected row again to deselect it.

The number of selected rows is obtained with the <a href="/package/extension5/sspread/properties/selectioncount">SelectionCount</a> property.
Get the selected line number with the <a href="/package/extension5/sspread/methods/getmultiselitem">GetMultiSelItem</a> method.
Use the <a href="/package/extension5/sspread/properties/selmodeselected">SelModeSelected</a> property to select rows from the CRS program.

### Extended Multiple Selection Mode ($ OperationModeExtended)
 
Operates as a list-type display control (multiple selection). Use this when you want to make both single selection and multiple selection.

The user cannot edit the cell. Focus does not move to individual cells.

Click a cell to select that row.
Multiple additional lines can be selected by holding down the [Ctrl] key and clicking.
A line range can be selected by holding down the [Shift] key and clicking.
Hold down the [Ctrl] key and click the selected line again to deselect it.

The number of selected rows is obtained with the <a href="/package/extension5/sspread/properties/selectioncount">SelectionCount</a> property.
Get the selected line number with the <a href="/package/extension5/sspread/methods/getmultiselitem">GetMultiSelItem</a> method.
Use the <a href="/package/extension5/sspread/properties/selmodeselected">SelModeSelected</a> property to select rows from the CRS program.

### Command button type and combo box type cells
 
In the row-by-row mode for spreadsheets (Row, Single, Multi, Extended), command buttons and combo boxes are not displayed. (The <a href="/package/extension5/sspread/properties/buttondrawmode">ButtonDrawMode</a>  property is also invalid.)

In row mode ($OperationModeRow), command buttons and combo boxes are displayed only when the row is in the edit state.
In read-only mode ($OperationModeRead), command buttons and combo boxes are visible but not available.

For command button type and combo box type cells, use in normal mode ($OperationModeNormal) or row mode ($OperationModeRow).

Related Items<br>
<a href="/package/extension5/sspread/properties/buttondrawmode">ButtonDrawMode</a>, <a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/selectioncount">SelectionCount</a>, <a href="/package/extension5/sspread/properties/selmodeindex">SelModeIndex</a>, <a href="/package/extension5/sspread/properties/selmodeselected">SelModeSelected</a> properties<br>
<a href="/package/extension5/sspread/methods/getmultiselitem">GetMultiSelItem</a> method<br>
<a href="/package/extension5/sspread/events/enterrow">EnterRow</a>, <a href="/package/extension5/sspread/events/leaverow">LeaveRow</a> events