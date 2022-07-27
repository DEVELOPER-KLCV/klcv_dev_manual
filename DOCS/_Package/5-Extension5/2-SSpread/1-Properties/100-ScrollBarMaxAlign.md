---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ScrollBarMaxAlign Property
nav_order: 100
permalink: /package/extension5/sspread/properties/scrollbarmaxalign
---
# {{ page.title }}

Sets the display position of the last cell when the spreadsheet is scrolled to the last row and column.

Specify the following values. The initial value is $TRUE.


| Constant | Description                                                        |
|----------|--------------------------------------------------------------------|
| $TRUE    | Display the last cell at the bottom right of the display area      |
| $FALSE   | Display the last cell in the upper left corner of the display area |

When scrolling to the end, $TRUE minimizes the gray area because the last cell is at the bottom right of the spreadsheet. In $FALSE, the area other than the last cell is gray.

Related Items<br>
<a href="/package/extension5/sspread/properties/grayareabackcolor">GrayAreaBackColor</a>, <a href="/package/extension5/sspread/properties/scrollbarwidth">ScrollBarWidth</a> properties 