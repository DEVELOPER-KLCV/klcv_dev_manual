---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.GetElementsByTagNameNS Method
nav_order: 12
permalink: /package/xmlpackage/xmldocument/methods/getelementsbytagnamens
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Search for Element nodes by namespace URI and tag name to get a list of matching Element nodes.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var list = xmldoc.GetElementsByTagNameNS( <b>namespaceURI, qualifiedName</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlNodeList object containing Element nodes that match the condition<br>If not found, an empty XmlNodeList object is returned.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>namespaceURI</b></td>
    <td>Namespace URI to search</td>
  </tr>
  <tr>
    <td>String <b>qualifiedName</b></td>
    <td>Tag name to search</td>
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
    var list = xmldoc.GetElementsByTagNameNS("http://www.w3.org/2000/svg", "rect");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnodelist">XmlNodeList</a>, <a href="/package/xmlpackage/xmlelement">XmlElement</a> classes<br><a href="/package/xmlpackage/xmldocument/methods/GetElementsByTagName">GetElementsByTagName</a>, <a href="/package/xmlpackage/xmldocument/methods/GetElementById">GetElementById</a> methods</td>
  </tr>
</table>



