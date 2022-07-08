---
layout: default

grand_parent: SSpread Class
parent: Operators
has_children: false
title: CSVDocument << SSpread Operator
nav_order: 2
permalink: /package/extension5/sspread/operators/2
---
# {{ page.title }}

This operator loads the SSpread object on the right side against the CSVDocument object on the left side.

Internally, the  <a href="/package/extension5/sspread/methods/exporttotextfile">ExportToTextFile</a> method is executed.
<br><small><span style="color:red">Added since Ver.5.0.2</span></small>

Example of usage

```
/* Save the contents of SSpread as CSV */
var csvdoc = new CSVDocument;
csvdoc << SSpread1;
var fs = new FileSystem;
var fp = fs.open("test.csv", FileSystem.OPEN_WRITE);
csvdoc.save(fp);
fp.close();
```
