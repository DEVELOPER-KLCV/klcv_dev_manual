---
layout: default

grand_parent: ListView Class
parent: Properties
has_children: false
title: ListView.Value Property
nav_order: 18
permalink: /package/extension4/listview/properties/value
---
# {{ page.title }}

The array number of the currently selected list item. Multiple items can be selected, but this will be the array number of the last item selected.

-1 indicates the non-selected state.

However, the value may be undefined when a row is inserted before the selected position or when a range is selected.

See the ListViewItem's index to get the correct row number. The line number can be obtained correctly by setting e.from.index in the Touch event of ListViewItem. 