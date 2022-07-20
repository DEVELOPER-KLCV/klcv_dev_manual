---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.CreateElementNS Method
nav_order: 7
permalink: /package/xmlpackage/xmldocument/methods/createelementns
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify the a namespace URI, then the Element node is created.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var elm = xmldoc.CreateElementNS( <b>namespaceURI, qualifiedName</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlElement object</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>namespaceURI</b></td>
    <td>Namespace URI of the Element node to be created</td>
  </tr>
  <tr>
    <td>String <b>qualifiedName</b></td>
    <td>Tag name of the Element node to be created</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>DOM-5</td>
    <td>INVALID_CHARACTER_ERR</td>
  </tr><tr>
    <td>DOM-14</td>
    <td>NAMESPACE_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var elm = xmldoc.CreateElementNS("http://www.w3.org/2000/svg", "svg:rect");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlelement">XmlElement</a> class<br><a href="/package/xmlpackage/xmldocument/methods/createelement">CreateElement</a> method</td>
  </tr>
</table>



