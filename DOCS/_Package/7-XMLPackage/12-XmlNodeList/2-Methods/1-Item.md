---
layout: default

grand_parent: XmlNodeList Class
parent: Methods
has_children: false
title: XmlNodeList.Item Method
nav_order: 1
permalink: /package/xmlpackage/xmlnodelist/methods/item
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Fetch the node by specifying the index.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node = list.Item( <b>index</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">	XmlNode object<br>If the corresponding node is not found, such as by specifying an <b>index</b> that is greater than or equal to the <a href="/package/xmlpackage/xmlnodelist/properties/length">Length</a> property , null is returned.
 </td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>index</b></td>
    <td>Position of the node to be retrieved ( by specifying an index starting from 0 )</td>
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
    for (var n = 0; n < list.Length; n++) {
        print(list.Item(n).NodeName, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode">XmlNode</a> class<br><a href="/package/xmlpackage/xmlnodelist/properties/length">Length</a> property<br><a href="">[ ]</a> operator</td>
  </tr>
</table>



