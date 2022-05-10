---
layout: default

grand_parent: XmlNodeList Class
parent: Methods
has_children: false
title: XmlNodeList.NextResetNode Method
nav_order: 3
permalink: /package/xmlpackage/xmlnodelist/methods/reset
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">list.Reset( )</td>
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
    var list = xmldoc.DocumentElement.ChildNodes;
    while (var n = list.NextNode()) {
        print(n.NodeName, "\n");
    }
    list.Reset();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnodelist/methods/nextnode">NextNode</a> method</td>
  </tr>
</table>



