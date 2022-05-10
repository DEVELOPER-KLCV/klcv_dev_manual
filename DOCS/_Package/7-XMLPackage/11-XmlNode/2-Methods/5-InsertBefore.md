---
layout: default

grand_parent: XmlNode Class
parent: Methods
has_children: false
title: XmlNode.InsertBefore Method
nav_order: 5
permalink: /package/xmlpackage/xmlnode/methods/InsertBefore
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node2 = node.InsertBefore( <b>newChild, refChild</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>XmlNode <b>newChild</b></td>
    <td></td>
  </tr>
  <tr>
    <td>XmlNode <b>refChild</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="4">Exception</td>
    <td>DOM-3</td>
    <td></td>
  </tr>
  <tr>
    <td>DOM-4</td>
    <td></td>
  </tr>
  <tr>
    <td>DOM-7</td>
    <td></td>
  </tr>
  <tr>
    <td>DOM-8</td>
    <td></td>
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
        var refChild = list.Item(n);
        if (refChild.NodeName == "C2") {
            var newChild = xmldoc.CreateElement("C1");
            parent.InsertBefore(newChild, refChild);
            break;
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmldocumentfragment">XmlDocumentFragment</a> class<br><a href="/package/xmlpackage/xmlnode/methods/replacechild">ReplaceChild</a>, <a href="/package/xmlpackage/xmlnode/methods/removechild">RemoveChild</a>, <a href="/package/xmlpackage/xmlnode/methods/appendchild">AppendChild</a> methods</td>
  </tr>
</table>



