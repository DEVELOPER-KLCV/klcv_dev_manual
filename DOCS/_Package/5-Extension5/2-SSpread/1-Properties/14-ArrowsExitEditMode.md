---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ArrowsExitEditMode Property
nav_order: 14
permalink: /package/extension5/sspread/properties/arrowsexiteditmode
---
# {{ page.title }}

Set the operation when the arrow keys are pressed in the cell whose input mode is ON (edited state).

Specify $TRUE to move to another cell, or $FALSE to move the cursor within the cell you are typing. The initial value is $FALSE.

If set to $FALSE, use the arrow keys to operate the cursor in the cell being edited. Ctrl + Arrow keys can be pressed to finish typing and move to the cell in that direction.

If set to $TRUE, use the arrow keys to move to the cell in that direction and finish typing. The cursor in a cell can be controlled by holding down the Ctrl key and pressing the arrow keys. 

Related Items <br>
<a href="/package/extension5/sspread/properties/editenteraction">EditEnterAction</a>, <a href="/package/extension5/sspread/properties/processtab">ProcessTab</a> property