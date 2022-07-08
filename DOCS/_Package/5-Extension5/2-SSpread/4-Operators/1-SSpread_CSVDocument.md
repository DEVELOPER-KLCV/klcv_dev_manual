---
layout: default

grand_parent: SSpread Class
parent: Operators
has_children: false
title: SSpread << CSVDocument Operator
nav_order: 1
permalink: /package/extension5/sspread/operators/1
---
# {{ page.title }}

This operator loads the CSVDocument object on the right side against the SSpread object on the left side.

The existing data will be deleted and replaced with the data in the CSVDocument object.

Internally, the <a href="/package/extension5/sspread/methods/loadtextfile">LoadTextFile</a> method is executed. <br><small><span style="color:red">Added since Ver.5.0.2</span></small>

Example of usage

```
/* Download CSV from the server and display it on SSpread */
var csvdoc = new CSVDocument;
csvdoc.get("test.csv");
SSpread1 << csvdoc;
 
 
/* Display CSV constants in SSpread */
SSpread1 << new CSVDocument << csv {
item1, item2, item3
item1, item2, item3
item1, item2, item3
item1, item2, item3
};
```
