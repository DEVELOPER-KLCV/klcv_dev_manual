---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.EditModeReplace Property
nav_order: 49
permalink: /package/extension5/sspread/properties/editmodereplace
---
# {{ page.title }}

Set whether to replace the entered value with the original value or add it to the original value when the input mode is turned ON.

Specify the following values. The initial value is $FALSE.

| Constant | Description                                                                                                                                                                                                                   |
|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| $TRUE    | Replace with original value <br> Select all cell contents when the input mode is turned ON. <br> When the input mode is turned ON by inputting characters, the contents of the cell are replaced with the entered characters. |
| $FALSE   | Add to the original value <br> Set the cursor at the end of the cell contents when the input mode is turned ON. <br> When the input mode is turned ON by inputting characters, it is added to the contents of the cell.       |

Related Item<br>
<a href="/package/extension5/sspread/properties/editmode">EditMode</a> property
