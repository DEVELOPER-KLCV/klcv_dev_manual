---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.RemoveAttributeNS Method
nav_order: 10
permalink: /package/xmlpackage/xmlelement/methods/removeattributens
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Delete the Attr node with the namespace URI and attribute name.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">elm.RemoveAttributeNS( <b>namespaceURI, name</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>namespaceURI</b></td>
    <td>Attr node namespace URI</td>
  </tr>
  <tr>
    <td>String <b>name</b></td>
    <td>Attr node attribute name</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>DOM-7</td>
    <td>NO_MODIFICATION_ALLOWED_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var elm = xmldoc.DocumentElement;
    elm.RemoveAttributeNS("http://www.w3.org/2000/svg", "style");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmlelement/methods/getattributens">GetAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributens">SetAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/hasattributens">HasAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattribute">RemoveAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattributenode">RemoveAttributeNode</a> method</td>
  </tr>
</table>



