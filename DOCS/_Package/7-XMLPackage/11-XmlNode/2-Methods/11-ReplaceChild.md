---
layout: default

grand_parent: XmlNode Class
parent: Methods
has_children: false
title: XmlNode.ReplaceChild Method
nav_order: 11
permalink: /package/xmlpackage/xmlnode/methods/ReplaceChild
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Swap child nodes.<br><small><span style="color:blue">Not supported in Mobile and AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node2 = node.ReplaceChild( <b>newChild, oldChild</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Swapped XmlNode object</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>XmlNode <b>newChild</b></td>
    <td>New node<br>If <b>newChild</b> is an <a href="/package/xmlpackage/xmldocumentfragment/">XmlDocumentFragment</a> object, all child nodes of <b>newChild</b> will be added in the same order. If <b>newChild</b> is connected to another tree, it will be inserted after being detached from the tree.</td>
  </tr>
  <tr>
    <td>Arguments</td>
    <td>XmlNode <b>oldChild</b></td>
    <td>Original child node</td>
  </tr>
  <tr>
    <td rowspan="4">Exception</td>
    <td>DOM-3</td>
    <td>HIERARCHY_REQUEST_ERR</td>
  </tr>
  <tr>
    <td>DOM-4</td>
    <td>WRONG_DOCUMENT_ERR</td>
  </tr>
  <tr>
    <td>DOM-7</td>
    <td>NO_MODIFICATION_ALLOWED_ERR</td>
  </tr>
  <tr>
    <td>DOM-8</td>
    <td>NOT_FOUND_ERR</td>
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
        var oldChild = list.Item(n);
        if (oldChild.NodeName == "C2") {
            var newChild = xmldoc.CreateElement("C1");
            parent.ReplaceChild(newChild, oldChild);
            break;
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmldocumentfragment">XmlDocumentFragment</a> class<br>,<a href="/package/xmlpackage/xmlnode/methods/insertbefore">InsertBefore</a>, <a href="/package/xmlpackage/xmlnode/methods/removechild">RemoveChild</a>, <a href="/package/xmlpackage/xmlnode/methods/appendchild">AppendChild</a> methods</td>
  </tr>
</table>



