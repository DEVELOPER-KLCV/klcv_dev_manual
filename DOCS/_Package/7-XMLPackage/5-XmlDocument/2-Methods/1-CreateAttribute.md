---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.CreateAttribute Method
nav_order: 1
permalink: /package/xmlpackage/xmldocument/methods/createattribute
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var attr = xmldoc.CreateAttribute( <b>name</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String  <b>name</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>DOM-5</td>
    <td>INVALID_CHARACTER_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var elm = xmldoc.CreateElement("rect");
    var attr = xmldoc.CreateAttribute("x");
    attr.Value = "10";
    elm.SetAttributeNode(attr);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmldocument/methods/createattributens">CreateAttributeNS</a> method</td>
  </tr>
</table>



