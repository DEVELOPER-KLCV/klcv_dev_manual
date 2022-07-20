---
layout: default

grand_parent: XmlDocument Class
parent: Operators
has_children: false
title: XmlDocument << XML Constant Operator
nav_order: 1
permalink: /package/xmlpackage/xmldocument/operators/1
---
# {{ page.title }}

This operator loads the <a href="/package/xmlpackage/xmldocument/constants">XML constants</a> on the right side of the XmlDocument object on the left side.

Example of use

```
var x = new XmlDocument ();
x << xml <<-
<? xml version = "1.0" encoding = "SHIFT_JIS"?>
<data>
    <record title = " Record 1 ">
        <item1> Item 1 </ item1>
        <item2> Item 1 </ item2>
        <item3> Item 1 </ item3>
    </ record>
</ data>
->>;
```