---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.SetAttributeNS Method
nav_order: 13
permalink: /package/xmlpackage/xmlelement/methods/setattributens
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">elm.SetAttributeNS( <b>namespaceURI, name, value </b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>String <b>namespaceURI</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>name</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>value</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>DOM-5</td>
    <td>INVALID_CHARACTER_ERR</td>
  </tr>
  <tr>
    <td>DOM-7</td>
    <td>NO_MODIFICATION_ALLOWED_ERR</td>
  </tr>
  <tr>
    <td>DOM-14</td>
    <td>NAMESPACE_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var elm = xmldoc.DocumentElement;
    elm.SetAttributeNS("http://www.w3.org/2000/svg ", "width", "100");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmlelement/methods/getattributens">GetAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattributens">RemoveAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/hasattributens">HasAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/setattribute">SetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributenode">SetAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributenodens">SetAttributeNodeNS</a> method</td>
  </tr>
</table>



