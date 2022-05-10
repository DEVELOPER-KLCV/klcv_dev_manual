---
layout: default

grand_parent: XmlNode Class
parent: Methods
has_children: false
title: XmlNode.SelectSingleNode Method
nav_order: 13
permalink: /package/xmlpackage/xmlnode/methods/selectsinglenode
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node2 = node.SelectSingleNode( <b>xpath</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>xpath</b></td>
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
    var node = xmldoc.DocumentElement.SelectSingleNode("//CODE");
    if (node != null) {
        print(node.NodeName, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode/methods/selectnodes">SelectNodes</a> method</td>
  </tr>
</table>



