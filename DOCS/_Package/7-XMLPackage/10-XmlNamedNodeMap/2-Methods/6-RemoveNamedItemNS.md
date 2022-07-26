---
layout: default

grand_parent: XmlNamedNodeMap Class
parent: Methods
has_children: false
title: XmlNamedNodeMap.RemoveNamedItemNS Method
nav_order: 6
permalink: /package/xmlpackage/xmlnamednodemap/methods/removenameditemns
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Delete the node by specifying the namespace URI and name.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node = map.RemoveNamedItemNS( <b>namespaceURI, name</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Deleted XmlNode object<br>Returns null if no node is found.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>namespaceURI</b></td>
    <td>Node namespace URI</td>
  </tr>
  <tr>
    <td>String <b>name</b></td>
    <td>Node name</td>
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
    map.RemoveNamedItemNS("http://www.w3.org/2000/svg", "width");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode">XmlNode</a> class<br><a href="/package/xmlpackage/xmlnamednodemap/methods/getnameditemns">GetNamedItemNS</a>, <a href="/package/xmlpackage/xmlnamednodemap/methods/setnameditemns">SetNamedItemNS</a>, <a href="/package/xmlpackage/xmlnamednodemap/methods/removenameditem">RemoveNamedItem</a> method</td>
  </tr>
</table>



