---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.AppearanceStyle Property
nav_order: 13
permalink: /package/extension5/sspread/properties/appearancestyle
---
# {{ page.title }}

Sets the design of the entire spreadsheet.

Specify the following values.

| Constant                     | Value | Description                                     |
|------------------------------|:-----:|-------------------------------------------------|
| $AppearanceStyleClassic      |   0   | Standard style <br>Standard design for Windows 2000 |
| $AppearanceStyleVisualStyles |   1   | Visual style <br>Standard design for Windows XP     |
| $AppearanceStyleEnhanced     |   2   | Extended style <br>Spreadsheet's unique design      |

The initial value depends on the OS setting and the <a href="/package/standard/displayobject/properties/visualstyle">DisplayObject.VisualStyle</a> property setting.

$AppearanceStyleClassic in the classic theme environment, $AppearanceStyle Enhanced otherwise.

The design of scroll bars, buttons placed in cells, checkboxes, etc. will also be changed.

Set the <a href="/package/extension5/sspread/properties/scrollbarstyle">ScrollBarStyle</a> property, to set the scrollbar design.

Set the <a href="/package/extension5/sspread/properties/usevisualstyles">UseVisualStyles</a> property, to set the design of the buttons and checkboxes placed in the cell. 

※ As a general rule, properties that set the spreadsheet design, such as this property, should be set first when the SSpread object is initialized. Programs that switch over and over while working with the spreadsheet are not recommended as they may temporarily misdraw the spreadsheet.

Related Items <br>
<a href="/package/extension5/sspread/properties/scrollbarstyle">ScrollBarStyle</a>, <a href="/package/extension5/sspread/properties/usevisualstyles">UseVisualStyles</a>, <a href="/package/extension5/sspread/properties/displayobjectvisualstyle">DisplayObject.VisualStyle</a> property