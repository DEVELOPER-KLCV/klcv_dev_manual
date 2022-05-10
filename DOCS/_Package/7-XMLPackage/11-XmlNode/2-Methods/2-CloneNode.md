---
layout: default

grand_parent: XmlNode Class
parent: Methods
has_children: false
title: XmlNode.CloneNode Method
nav_order: 2
permalink: /package/xmlpackage/xmlnode/methods/clonenode
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node2 = node.CloneNode( <b>deep</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>boolean <b>deep</b></td>
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
    var parent = xmldoc.DocumentElement;
    var list = parent.ChildNodes;
    for (var n in list) {
        var node = list.Item(n);
        if (node.NodeName == "C1") {
            var node2 = node1.CloneNode(true);
            parent.AppendChild(node2);
            break;
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmldocument">XmlDocument</a> class</td>
  </tr>
</table>



