---
layout: default

grand_parent: ListView Class
parent: Properties
has_children: false
title: ListView.ColHeader Property
nav_order: 6
permalink: /package/extension4/listview/properties/colheader
---
# {{ page.title }}

The operation of the column. Only ListStyle = $REPORT is valid.

Sorting depends on the data type set for the column. If the column header is pressed while sorting is possible, it will be sorted and will change in the order of creation → descending order ▽ → ascending order △.

| Constant    | Value | Description                                              |
|-------------|:-----:|----------------------------------------------------------|
| $STD        |   0   | Column click enabled, column cannot be moved             |
| $MOVE       |   1   | Column click enabled, column can be moved by dragging    |
| $NOSORT     |   2   | Column click prohibited, column cannot be moved          |
| $NOSORTMOVE |   3   | Column click prohibited, column can be moved by dragging |
| $NOCOLUMN   |   4   | Hide column                                              |