---
layout: default

grand_parent: XmlNodeList Class
parent: Methods
has_children: false
title: XmlNodeList.NextNode Method
nav_order: 2
permalink: /package/xmlpackage/xmlnodelist/methods/nextnode
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Take out the next node.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node = list.NextNode( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlNode object<br>Return null if no more nodes are found.</td>
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
    var list = xmldoc.DocumentElement.ChildNodes;
    while (var n = list.NextNode()) {
        print(n.NodeName, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode">XmlNode</a> class<br><a href="/package/xmlpackage/xmlnodelist/methods/reset">Reset</a> method</td>
  </tr>
</table>



