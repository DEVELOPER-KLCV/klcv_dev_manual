---
layout: default

grand_parent: XmlNamedNodeMap Class
parent: Methods
has_children: false
title: XmlNamedNodeMap.GetNamedItemNS Method
nav_order: 2
permalink: /package/xmlpackage/xmlnamednodemap/methods/getnameditemns
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node = map.GetNamedItemNS( <b>namespaceURI, localName</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>namespaceURI</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>localName</b></td>
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
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var map = xmldoc.DocumentElement.Attributes;
    var attr = map.GetNamedItemNS("http://www.w3.org/2000/svg", "x");
    print(attr.NodeValue, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode">XmlNode</a> class<br><a href="/package/xmlpackage/xmlnamednodemap/methods/setnameditemns">SetNamedItemNS</a>, <a href="/package/xmlpackage/xmlnamednodemap/methods/removenameditemns">RemoveNamedItemNS</a>, <a href="/package/xmlpackage/xmlnamednodemap/methods/getnameditem">GetNamedItem</a> method</td>
  </tr>
</table>



