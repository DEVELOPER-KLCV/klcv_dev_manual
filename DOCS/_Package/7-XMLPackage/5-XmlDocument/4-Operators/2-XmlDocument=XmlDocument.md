---
layout: default

grand_parent: XmlDocument Class
parent: Operators
has_children: false
title: XmlDocument << XmlDocument Operator
nav_order: 2
permalink: /package/xmlpackage/xmldocument/operators/2
---
# {{ page.title }}

This operator copies the XmlDocument on the right side to the XmlDocument object on the left side .

Example of use

```
var impl = new XmlDOMImplementation;
var res = GetHttpSession (). Get ("sample.xml");
var xml1 = impl.Load (res);
 
var xml2 = new XmlDocument ();
xml2 << xml1;
```