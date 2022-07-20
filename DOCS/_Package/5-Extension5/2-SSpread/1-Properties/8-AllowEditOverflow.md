---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.AllowEditOverflow Property
nav_order: 8
permalink: /package/extension5/sspread/properties/alloweditoverflow
---
# {{ page.title }}

When the input mode is ON (the active cell is in the editing state), if the character string being input is larger than the cell width, set whether to display it in the adjacent cell.

Specify $TRUE if it is displayed outside, and $FALSE otherwise.

The initial value is $FALSE. 
If the cell is left-aligned, it extends to the right cell, and if it is right-aligned, it extends to the left cell. If it is centered, it will stick out to the cells on both sides.

If a value is set in the next cell that extends beyond, that cell will be temporarily hidden until the input mode is turned off. (The character string being entered has priority)

Related Item<br>
<a href="/package/extension5/sspread/properties/allowcelloverflow">AllowCellOverflow</a>, <a href="/package/extension5/sspread/properties/editmode">EditMode</a> property<br>