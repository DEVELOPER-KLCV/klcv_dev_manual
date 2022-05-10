---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.GetAttributeNode Method
nav_order: 3
permalink: /package/xmlpackage/xmlelement/methods/getattributenode
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var attr = elm.GetAttributeNode( <b>name</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
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
    var attr = elm.GetAttributeNode("width");
    print(attr.Value, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmlelement/methods/setattributenode">SetAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattributenode">RemoveAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/hasattribute">HasAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/getattribute">GetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributens">GetAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/getattributenodens">GetAttributeNodeNS</a> method</td>
  </tr>
</table>



