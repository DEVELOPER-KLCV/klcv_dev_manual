---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.GetAttribute Method
nav_order: 1
permalink: /package/xmlpackage/xmlelement/methods/getattribute
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Get the value of the Attr node with the specified attribute name .</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = elm.GetAttribute( <b>name</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Value of Attr node string<br>If the Attr node is not found, it returns an empty string.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>name</b></td>
    <td>get the value of attribute name of the Attr node </td>
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
    var s = elm.GetAttribute("width");
    print(s, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmlelement/methods/setattribute">SetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattribute">RemoveAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/hasattribute">HasAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributenode">GetAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributens">GetAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributenodens">GetAttributeNodeNS</a> method</td>
  </tr>
</table>



