---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.AllowCellOverflow Property
nav_order: 5
permalink: /package/extension5/sspread/properties/allowcelloverflow
---
# {{ page.title }}

Set whether to display in the adjacent cell when the character string set in the cell is larger than the width of the cell.

Specify $TRUE if it is displayed outside, and $FALSE otherwise. The initial value is $FALSE.

If the cell is left-aligned, it extends to the right cell, and if it is right-aligned, it extends to the left cell. If it is centered, it will stick out to the cells on both sides.

If a value is set in the cell next to the cell, the value in that cell is displayed with priority, so it does not extend.

Related Item <br>
<a href="/package/extension5/sspread/properties/alloweditoverflow">AllowEditOverflow</a> property<br>