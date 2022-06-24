---
layout: default

grand_parent: FlexView Class
parent: Operators
has_children: false
title: CSVDocument << FlexView Operator
nav_order: 2
permalink: /package/extension4/flexview/flexview/operators/2
---
# {{ page.title }}

This operator loads a FlexView object on the right side of the CSVDocument object on the left side.

The CSVDocument column corresponds to the Value property of the FlexData-derived class.

Usage example

```
/* FlexViewの内容をCSVで保存する */
var csvdoc = new CSVDocument;
csvdoc << FlexView1;
var fs = new FileSystem;
var fp = fs.open("test.csv", FileSystem.OPEN_WRITE);
csvdoc.save(fp);
fp.close();
```

