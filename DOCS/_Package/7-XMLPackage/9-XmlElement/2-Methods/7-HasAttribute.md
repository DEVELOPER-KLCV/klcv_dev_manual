---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.HasAttribute Method
nav_order: 7
permalink: /package/xmlpackage/xmlelement/methods/hasattribute
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Checks if there is an Attr node with the specified attribute name.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = elm.HasAttribute( <b>name</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">$TRUE if the Attr node exists , $FALSE if it does not exist</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>name</b></td>
    <td>Attribute name</td>
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
    var ret = elm.HasAttribute("style");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlelement/methods/hasattributens">HasAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/getattribute">GetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/setattribute">SetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattribute">RemoveAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributenode">GetAttributeNode</a> method</td>
  </tr>
</table>



