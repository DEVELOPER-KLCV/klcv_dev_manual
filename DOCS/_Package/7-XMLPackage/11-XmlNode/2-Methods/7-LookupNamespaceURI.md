---
layout: default

grand_parent: XmlNode Class
parent: Methods
has_children: false
title: XmlNode.LookupNamespaceURI Method
nav_order: 7
permalink: /package/xmlpackage/xmlnode/methods/LookupNamespaceURI
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the namespace URI that corresponds to the specified prefix.<br><small><span style="color:red">Added since Ver.4.0.0</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var namespaceURI = node.LookupNamespaceURI( <b>prefix</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Corresponding namespace URI<br>Returns null if not found.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>prefix</b></td>
    <td>Namespace URI prefix</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var namespaceURI = node.LookupNamespaceURI("svg");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnode/properties/namespaceuri">NamespaceURI</a>, <a href="/package/xmlpackage/xmlnode/properties/prefix">Prefix</a> properties<br><a href="/package/xmlpackage/xmlnode/methods/lookupprefix">LookupPrefix</a> method</td>
  </tr>
</table>



