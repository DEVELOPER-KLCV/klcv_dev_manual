---
layout: default

grand_parent: XmlNamedNodeMap Class
parent: Methods
has_children: false
title: XmlNamedNodeMap.SetNamedItemNS Method
nav_order: 9
permalink: /package/xmlpackage/xmlnamednodemap/methods/setnameditemns
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify the <a href="/package/xmlpackage/xmlnode">XmlNode</a> object to set the node.<br>If a node with the same namespace URI and name as the specified node is already included in the node map, that node will be replaced.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node = map.SetNamedItemNS( <b>newNode</b> )</td>
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
    var attr = dom.CreateAttributeNS("http://www.w3.org/2000/svg", "width");
    attr.Value = "10";
    map.SetNamedItemNS(attr);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode">XmlNode</a> class<br><a href="/package/xmlpackage/xmlnamednodemap/methods/getnameditemns">GetNamedItemNS</a>, <a href="/package/xmlpackage/xmlnamednodemap/methods/removenameditemns">RemoveNamedItemNS</a>, <a href="/package/xmlpackage/xmlnamednodemap/methods/setnameditem">SetNamedItem</a> method</td>
  </tr>
</table>



