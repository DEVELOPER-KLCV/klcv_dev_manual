---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.SetAttributeNodeNS Method
nav_order: 15
permalink: /package/xmlpackage/xmlelement/methods/setattributenodens
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify the<a href="/package/xmlpackage/xmlattr/"> XmlAttr</a>object to configure the Attr node.<br>If there is an Attr node with the same namespace URI and attribute name as the specified XmlAttr object, it will replace the Attr node.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var attr2 = elm.SetAttributeNodeNS( <b>attr</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Replaced XmlAttr object<br>Returns null if there was no replacement.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>XmlAttr <b>attr</b></td>
    <td>XmlAttr object to be set<br>An Attr node that has already been set to another Element node cannot be specified.</td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>DOM-4</td>
    <td>WRONG_DOCUMENT_ERR</td>
  </tr>
  <tr>
    <td>DOM-7</td>
    <td>NO_MODIFICATION_ALLOWED_ERR</td>
  </tr>
  <tr>
    <td>DOM-10</td>
    <td>INUSE_ATTRIBUTE_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var elm = xmldoc.DocumentElement;
    var attr = elm.GetAttributeNodeNS("http://www.w3.org/2000/svg", "width");
    var attr2 = attr.CloneNode($TRUE);
    elm.SetAttributeNodeNS(attr2);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmlelement/methods/getattributenodens">GetAttributeNodeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/setattribute">SetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributenode">SetAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributens">SetAttributeNS</a> method</td>
  </tr>
</table>



