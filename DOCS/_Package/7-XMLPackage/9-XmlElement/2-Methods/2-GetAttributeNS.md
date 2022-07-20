---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.GetAttributeNS Method
nav_order: 2
permalink: /package/xmlpackage/xmlelement/methods/getattributens
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Get the value of the Attr node for the specified namespace URI and attribute name.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = elm.GetAttributeNS( <b>namespaceURI, name </b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Attr node value string.If the Attr node is not found, an empty string is returned.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>namespaceURI</b></td>
    <td>Namespace URI of the Attr node for which you want to get the value</td>
  </tr>
  <tr>
    <td>String <b>name</b></td>
    <td>Attribute name of the Attr node for which you want to get the value</td>
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
    var s = elm.GetAttributeNS("http://www.w3.org/2000/svg ", "width");
    print(s, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmlelement/methods/setattributens">SetAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattributens">RemoveAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/hasattributens">HasAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/getattribute">GetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributeNode">GetAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributenodens">GetAttributeNodeNS</a> method</td>
  </tr>
</table>



