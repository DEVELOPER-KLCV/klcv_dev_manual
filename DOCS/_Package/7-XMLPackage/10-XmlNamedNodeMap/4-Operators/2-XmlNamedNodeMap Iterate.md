---
layout: default

grand_parent: XmlNamedNodeMap Class
parent: Operators
has_children: false
title: XmlNamedNodeMap Iterate Operator
nav_order: 2
permalink: /package/xmlpackage/xmlnamednodemap/operators/2
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Eject nodes in continously.<br>The Iterate operator, unlike a normal operator, is used to continuously access the data contained in an object inside the execution engine. Objects with Iterate can perform the same operations as arrayed objects with <a href="/bizBrowserV/3/3-14/">for in loops</a> and <a href="/method/statistical/sum">sum</a> functions.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">The Iterate operator cannot be called directly.</td>
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
    var map = xmldoc.DocumentElement.Attributes;
    for (var n in map) {
        print(map[n].NodeName, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode">XmlNode</a> class</td>
  </tr>
</table>



