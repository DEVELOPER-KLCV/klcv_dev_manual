---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.RemoveAttribute Method
nav_order: 9
permalink: /package/xmlpackage/xmlelement/methods/removeattribute
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Delete the Attr node by specifying the attribute name .<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">elm.RemoveAttribute( <b>name</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
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
    elm.RemoveAttribute("style");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmlelement/methods/getattribute">GetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/setattribute">SetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/hasattribute">HasAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattributenode">RemoveAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattributens">RemoveAttributeNS</a> method</td>
  </tr>
</table>



