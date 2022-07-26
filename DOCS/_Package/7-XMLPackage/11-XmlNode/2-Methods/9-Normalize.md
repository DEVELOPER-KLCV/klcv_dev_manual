---
layout: default

grand_parent: XmlNode Class
parent: Methods
has_children: false
title: XmlNode.Normalize Method
nav_order: 9
permalink: /package/xmlpackage/xmlnode/methods/normalize
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Normalizes the Text node.<br><br>Empty Text nodes are deleted and adjacent Text nodes are concatenated into a single Text node.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">node.Normalize( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
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
    var parent = xmldoc.DocumentElement;
    parent.AppendChild(xmldoc.CreateTextNode("aaaaa\n"));
    parent.AppendChild(xmldoc.CreateTextNode("bbbbb\n"));
    parent.AppendChild(xmldoc.CreateTextNode("ccccc\n"));
    parent.Normalize();
    xmldoc.Save(file);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmltext">XmlText</a> class</td>
  </tr>
</table>



