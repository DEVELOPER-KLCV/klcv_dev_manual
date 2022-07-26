---
layout: default

grand_parent: XmlNodeList Class
parent: Operators
has_children: false
title: XmlNodeList Iterate Operator
nav_order: 2
permalink: /package/xmlpackage/xmlnodelist/operators/2
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Eject nodes in succession.<br>The Iterate operator is unlike a normal operator, and is used to continuously access the data contained in an object inside the execution engine. Class objects  with Iterate can perform the same operations as arrayed objects with for <a href="/bizBrowserV/3/3-14/">for in loops</a> and <a href="/method/statistical/sum">sum</a> functions.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">Iterate operator cannot be called directly.</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Iterate object</td>
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
    for (var n in list) {
        print(nodeList[n].nodeName, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode">XmlNode</a> class</td>
  </tr>
</table>



