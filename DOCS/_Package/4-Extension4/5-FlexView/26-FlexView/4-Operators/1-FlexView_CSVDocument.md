---
layout: default

grand_parent: FlexView Class
parent: Operators
has_children: false
title: FlexView << CSVDocument Operator
nav_order: 1
permalink: /package/extension4/flexview/flexview/operators/1
---
# {{ page.title }}

This operator loads a CSVDocument object on the right side of the FlexView object on the left side.

The existing data will be deleted and replaced with the data in the CSVDocument object.

If even one column name is defined in CSVDocument, it will be assigned to the corresponding FlexData in FlexView. If there is a mixture of anonymous columns, the anonymous columns will be ignored.

If no column name is defined in CSVDocument, it will be assigned to the corresponding FlexData in FlexView in the order of CSVDocument.

Usage example

```
/* CSVをサーバからダウンロード後FlexViewへ表示する */
var csvdoc = new CSVDocument;
csvdoc.get("test.csv");
FlexView1 << csvdoc;
 
 
/* CSV定数をFlexViewへ表示する */
FlexView1 << new CSVDocument << csv {
item1, item2, item3
item1, item2, item3
item1, item2, item3
item1, item2, item3
};
```

