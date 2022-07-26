---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.GetAttributeNodeNS Method
nav_order: 4
permalink: /package/xmlpackage/xmlelement/methods/getattributenodens
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Get the Attr node by specifying the namespace URI and attribute name.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var attr = elm.GetAttributeNodeNS( <b>namespaceURI, name </b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlAttr object<br>Returns null if not found.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>namespaceURI</b></td>
    <td>Namespace URI of Attr node</td>
  </tr>
  <tr>
    <td>String <b>name</b></td>
    <td>Attr node attribute name</td>
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
    var attr = elm.GetAttributeNodeNS("http://www.w3.org/2000/svg", "width");
    print(attr.Value, "\n");   
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmlelement/methods/setattributenodens">SetAttributeNodeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/hasattributens">HasAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/getattribute">GetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributenode">GetAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributens">GetAttributeNS</a> method</td>
  </tr>
</table>



