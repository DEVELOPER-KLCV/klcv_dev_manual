---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.ImportNode Method
nav_order: 13
permalink: /package/xmlpackage/xmldocument/methods/importnode
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Import the node from another DOM tree.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var cnode = xmldoc.ImportNode( <b>node, deep</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Imported XmlNode object<br>This node is not yet connected to the document tree and has no parent.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>XmlNode <b>node</b></td>
    <td>Node to import</td>
  </tr>
  <tr>
    <td>boolean <b>deep</b></td>
    <td>$TRUE for recursive imports , $FALSE otherwise</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>DOM-9</td>
    <td>NOT_SUPPORTED_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var orgnode = xmldocA.DocumentElement.FirstChild;
    var copynode = xmldocB.ImportNode(orgnode, $TRUE);
    xmldocB.DocumentElement.FirstChild.AppendChild(copynode);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmldocument">XmlDocument</a>, <a href="/package/xmlpackage/xmlnode">XmlNode</a> classes</td>
  </tr>
</table>



