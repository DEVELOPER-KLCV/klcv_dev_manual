---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.HasAttributeNS Method
nav_order: 8
permalink: /package/xmlpackage/xmlelement/methods/hasattributens
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = elm.HasAttributeNS( <b>namespaceURI, name </b> )</td>
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
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var elm = xmldoc.DocumentElement;
    var ret = elm.HasAttributeNS("http://www.w3.org/2000/svg", "style");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlelement/methods/hasattribute">HasAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributens">GetAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributens">SetAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattributens">RemoveAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributenodens">GetAttributeNodeNS</a> method</td>
  </tr>
</table>



