---
layout: default

grand_parent: XmlNamedNodeMap Class
parent: Methods
has_children: false
title: XmlNamedNodeMap.SetNamedItem Method
nav_order: 8
permalink: /package/xmlpackage/xmlnamednodemap/methods/setnameditem
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify the <a href="/package/xmlpackage/xmlnode">XmlNode</a> object to set the node.<br>If the node map already contains a node with the same name as the specified node, that node will be replaced.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node = map.SetNamedItem( <b>newNode</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Replaced XmlNode object<br>Returns null if the replacement did not occur .</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>XmlNode <b>newNode</b></td>
    <td>Node to be set</td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>DOM-4</td>
    <td>WRONG_DOCUMENT_ERR</td>
  </tr>
  <tr>
    <td>DOM-7</td>
    <td>NO_MODIFICATION_ALLOWED_ERR</td>
  </tr>
  
  <tr>
    <td>DOM-10</td>
    <td>INUSE_ATTRIBUTE_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var map = xmldoc.DocumentElement.Attributes;
    var attr = xmldoc.CreateAttribute("width");
    attr.Value = "10";
    map.SetNamedItem(attr);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode">XmlNode</a> class<br><a href="/package/xmlpackage/xmlnamednodemap/methods/getnameditem">GetNamedItem</a>, <a href="/package/xmlpackage/xmlnamednodemap/methods/removenameditem">RemoveNamedItem</a>, <a href="/package/xmlpackage/xmlnamednodemap/methods/setnameditemns">SetNamedItemNS</a> method<br><a href="package/xmlpackage/xmlnamednodemap/operators/1">[ ] </a> operator</td>
  </tr>
</table>



