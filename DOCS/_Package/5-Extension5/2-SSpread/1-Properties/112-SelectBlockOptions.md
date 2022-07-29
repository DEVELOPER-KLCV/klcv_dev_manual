---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.SelectBlockOptions Property
nav_order: 112
permalink: /package/extension5/sspread/properties/selectblockoptions
---
# {{ page.title }}

Sets the types of cell blocks that can be selected.

Specify a combination of the following values. The initial value is 15 (all combinations below).

| Constant                   | Value | Description                                                                    |
|----------------------------|:-----:|--------------------------------------------------------------------------------|
| $SelectBlockOptionsColumns |   1   | Column selection <br> Click the column header to select the entire column      |
| $SelectBlockOptionsRows    |   2   | Row selection <br> Click the row header to select the entire row               |
| $SelectBlockOptionsBlocks  |   4   | Cell block selection <br> Drag a cell to select a range of cells                    |
| $SelectBlockOptionsAll     |   8   | Select all <br> Click on the top left corner of the spreadsheet to select the whole |

Example of usage<br>
```
SelectBlockOptions = $SelectBlockOptionsColumns + $SelectBlockOptionsRows;
```
