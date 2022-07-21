---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.EditEnterAction Property
nav_order: 46
permalink: /package/extension5/sspread/properties/editenteraction
---
# {{ page.title }}

Set the operation when the Enter key is pressed.

Specify the following values. The initial value is $EditEnterActionNone.

| Constant                 | Value | Description                                                                                                   |
|--------------------------|:-----:|---------------------------------------------------------------------------------------------------------------|
| $EditEnterActionNone     |   0   | Turn on input mode without moving the active cell                                                             |
| $EditEnterActionUp       |   1   | Move active cell to upper cell                                                                                |
| $EditEnterActionDown     |   2   | Move active cell to lower cell                                                                                |
| $EditEnterActionLeft     |   3   | Move active cell to left cell                                                                                 |
| $EditEnterActionRight    |   4   | Move active cell to right cell                                                                                |
| $EditEnterActionNext     |   5   | Move active cell to right cell <br> If it is the last column, move to the first column of the next row        |
| $EditEnterActionPrevious |   6   | Move active cell to previous cell <br> If it is the first column, move to the last column of the previous row |
| $EditEnterActionSame     |   7   | Same as $EditEnterActionNone                                                                                  |
| $EditEnterActionNextRow  |   8   | Move active cell to first column of next row                                                                  |

If press the Enter key in a cell whose input mode is ON (edit mode), it will move to the cell set in this property after the input mode is turned OFF.

Related Item<br>
<a href="/package/extension5/sspread/properties/arrowsexiteditmode">ArrowsExitEditMode</a>, <a href="/package/extension5/sspread/properties/processtab">ProcessTab</a> property 