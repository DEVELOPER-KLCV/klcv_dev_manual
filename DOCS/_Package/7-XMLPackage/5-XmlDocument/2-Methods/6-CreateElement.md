---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.CreateElement Method
nav_order: 6
permalink: /package/xmlpackage/xmldocument/methods/createelement
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Create an Element node.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var elm = xmldoc.CreateElement( <b>tagName</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlElement object</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>tagName</b></td>
    <td>Tag name of the Element node to be created</td>
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
    var elm = xmldoc.CreateElement("TAG1");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlelement">XmlElement</a> class<br><a href="/package/xmlpackage/xmldocument/methods/createelementns">CreateElementNS</a> method</td>
  </tr>
</table>



