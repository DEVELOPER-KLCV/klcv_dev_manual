---
layout: default

grand_parent: FlexView Class
parent: Properties
has_children: false
title: FlexView.RowPosition Property
nav_order: 16
permalink: /package/extension4/flexview/flexview/properties/rowposition
---
# {{ page.title }}

Indicates the currently selected row position.

When the cursor moves over the FlexTreeHeader, the row is different on the display, but the RowPosition has the same value as the first row pointed to by the FlexTreeHeader.

If no row is selected, it will be -1.

If you specify a line that is folded and not displayed by FlexTreeHeader, the specified line is unfolded and displayed on the screen.

If you specify a value other than the existing row, the exception, Ext-13, will occur.