---
layout: default

grand_parent: XmlNamedNodeMap Class
parent: Operators
has_children: false
title: XmlNamedNodeMap[ ] Operator
nav_order: 1
permalink: /package/xmlpackage/xmlnamednodemap/operators/1
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">map[ <b>name</b> ]</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>name</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var map = xmldoc.DocumentElement.Attributes;
    print(map["width"].NodeName, "\n");
    map["width"].NodeValue = "100";
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode">XmlNode</a> class<br><a href="/package/xmlpackage/xmlnamednodemap/methods/getnameditem">GetNamedItem</a>, <a href="/package/xmlpackage/xmlnamednodemap/methods/setnameditem">SetNamedItem</a> methods</td>
  </tr>
</table>



