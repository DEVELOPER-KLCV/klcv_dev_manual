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
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node = map.SetNamedItemNS( <b>newNode</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>XmlNode <b>newNode</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>DOM-4</td>
    <td></td>
  </tr>
  <tr>
    <td>DOM-7</td>
    <td></td>
  </tr>
  
  <tr>
    <td>DOM-10</td>
    <td></td>
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



