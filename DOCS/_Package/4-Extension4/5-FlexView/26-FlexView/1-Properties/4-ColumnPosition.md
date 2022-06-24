---
layout: default

grand_parent: FlexView Class
parent: Properties
has_children: false
title: FlexView.ColumnPosition Property
nav_order: 4
permalink: /package/extension4/flexview/flexview/properties/columnposition
---
# {{ page.title }}

Indicates the currently selected column position. The column positions are 0,1,2 ... in the order of definition (from the left), except for columns configured by FlexHeader and derived classes.

If the cursor moves over FlexTreeHeader, it retains its previous value.

If no column is selected, it will be -1.

If you specify a value other than an existing column, the exception, Ext-14, will occur.

 