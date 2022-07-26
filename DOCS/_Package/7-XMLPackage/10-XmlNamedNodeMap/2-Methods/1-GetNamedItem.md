---
layout: default

grand_parent: XmlNamedNodeMap Class
parent: Methods
has_children: false
title: XmlNamedNodeMap.GetNamedItem Method
nav_order: 1
permalink: /package/xmlpackage/xmlnamednodemap/methods/getnameditem
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Fetch the node by name.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node = map.GetNamedItem( <b>name</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlNode object<br>Returns null if no node is found.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
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
    print(map.GetNameItem("width").NodeValue, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode">XmlNode</a> class<br><a href="/package/xmlpackage/xmlnamednodemap/methods/setnameditem">SetNamedItem</a>, <a href="/package/xmlpackage/xmlnamednodemap/methods/removenameditem">RemoveNamedItem</a>, <a href="/package/xmlpackage/xmlnamednodemap/methods/getnameditemns">GetNamedItemNS</a> method<br><a href="/package/xmlpackage/xmlnamednodemap/operators/1">[ ]</a> operator</td>
  </tr>
</table>



