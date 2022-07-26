---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.RemoveAttributeNode Method
nav_order: 11
permalink: /package/xmlpackage/xmlelement/methods/removeattributenode
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Delete the Attr node by specifying the<a href="/package/xmlpackage/xmlattr/">XmlAttr</a>.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">elm.RemoveAttributeNode( <b>attr</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Deleted XmlAttr object.Returns null if it was not deleted .</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>XmlAttr <b>attr</b></td>
    <td>XmlAttr object to delete</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>DOM-7</td>
    <td>NO_MODIFICATION_ALLOWED_ERR</td>
  </tr>
  <tr>
    <td>DOM-8</td>
    <td>NOT_FOUND_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var elm = xmldoc.DocumentElement;
    var attr = elm.GetAttributeNode("width");
    elm.RemoveAttributeNode(attr);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlattr">XmlAttr</a> class<br><a href="/package/xmlpackage/xmlelement/methods/getattributenode">GetAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/setattributenode">SetAttributeNode</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattribute">RemoveAttribute</a>, <a href="/package/xmlpackage/xmlelement/methods/removeattributens">RemoveAttributeNS</a> methods</td>
  </tr>
</table>



