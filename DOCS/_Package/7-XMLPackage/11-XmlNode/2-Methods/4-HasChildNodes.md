---
layout: default

grand_parent: XmlNode Class
parent: Methods
has_children: false
title: XmlNode.HasChildNodes Method
nav_order: 4
permalink: /package/xmlpackage/xmlnode/methods/haschildnodes
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Check for the existence of child nodes.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = node.HasChildNodes( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">$TRUE if there are child nodes , $FALSE if not</td>
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
    if (parent.HasChildNodes()) {
        var list = parent.ChildNodes;
        for (var n in list) {
            print(list.Item(n).NodeName, "\n");
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode/properties/childnodes">ChildNodes</a> property</td>
  </tr>
</table>



