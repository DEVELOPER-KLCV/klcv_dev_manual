---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.SetAttribute Method
nav_order: 12
permalink: /package/xmlpackage/xmlelement/methods/setattribute
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">elm.SetAttribute( <b>name, value</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>name</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>value</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>DOM-5</td>
    <td>INVALID_CHARACTER_ERR</td>
  </tr>
  <tr>
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
    elm.SetAttribute("width", "100");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmlelement/methods/getattribute">GetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattribute">RemoveAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/hasattribute">HasAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributenode">SetAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributens">SetAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributenodens">SetAttributeNodeNS</a> method</td>
  </tr>
</table>



