---
layout: default

grand_parent: XmlNamedNodeMap Class
parent: Methods
has_children: false
title: XmlNamedNodeMap.Item Method
nav_order: 3
permalink: /package/xmlpackage/xmlnamednodemap/methods/item
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Fetch the node by specifying the index.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node = map.Item( <b>index</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlNode object<br>If the corresponding node is not found, such as by specifying an <b>index</b> that is greater than or equal to the <a href="/package/xmlpackage/xmlnamednodemap/properties/length">Length</a> property , null is returned.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>index</b></td>
    <td>Position of the node to retrieve ( by specifying an index starting from 0 )</td>
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
    for (var n = 0; n < map.Length; n++) {
        print(map.Item(n).NodeName, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode">XmlNode</a> class<br><a href="/package/xmlpackage/xmlnamednodemap/properties/length">Length</a> property</td>
  </tr>
</table>



