---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.SetAttributeNode Method
nav_order: 14
permalink: /package/xmlpackage/xmlelement/methods/setattributenode
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify the<a href="/package/xmlpackage/xmlattr/"> XmlAttr</a>object to configure the Attr node.<br>If there is an Attr node with the same attribute name as the specified XmlAttr object, replace the Attr node.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var attr2 = elm.SetAttributeNode( <b>attr</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Replaced XmlAttr object.<br>Returns null if there was no replacement.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>XmlAttr <b>attr</b></td>
    <td>XmlAttr object to be set<br>You cannot specify an Attr node that is already set on another Element node.</td>
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
    var attr = elm.GetAttributeNode("width");
    var attr2 = attr.CloneNode(true);
    elm.SetAttributeNode(attr2);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmlelement/methods/getattributenode">GetAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattributeNode">RemoveAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/setattribute">SetAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributens">SetAttributeNS</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributenodens">SetAttributeNodeNS</a> method</td>
  </tr>
</table>



