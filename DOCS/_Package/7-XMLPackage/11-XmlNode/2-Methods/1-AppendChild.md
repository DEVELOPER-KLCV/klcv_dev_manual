---
layout: default

grand_parent: XmlNode Class
parent: Methods
has_children: false
title: XmlNode.AppendChild Method
nav_order: 1
permalink: /package/xmlpackage/xmlnode/methods/appendchild
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node2 = node.AppendChild( <b>child</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>XmlNode <b>child</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>DOM-3</td>
    <td></td>
  </tr>
  <tr>
    <td>DOM-7</td>
    <td></td>
  </tr>
  <tr>
    <td>DOM-8</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var parent = xmldoc.DocumentElement;
    var child = xmldoc.CreateElement("C3");
    parent.AppendChild(child);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode/methods/insertbefore">InsertBefore</a>, <a href="/package/xmlpackage/xmlnode/methods/replacechild">ReplaceChild</a>, <a href="/package/xmlpackage/xmlnode/methods/removechild">RemoveChild</a> methods</td>
  </tr>
</table>



