---
layout: default

grand_parent: XmlDOMImplementation Class
parent: Methods
has_children: false
title: XmlDOMImplementation Constructor
nav_order: 1
permalink: /package/xmlpackage/xmldomimplementation/methods/constructor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var domimpl = new XmlDOMImplementation( [ <b>enc</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>enc</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation(XmlDOMImplementation.Unicode);
    var xmldoc = domimpl.CreateDocument(NULL, “data”, NULL);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmldocument">XmlDocument</a> class<br><a href="/package/xmlpackage/xmldomimplementation/methods/createdocument">CreateDocument</a>, <a href="/package/xmlpackage/xmldomimplementation/methods/parse">Parse</a>, <a href="/package/xmlpackage/xmldomimplementation/methods/load">Load</a> method</td>
  </tr>
</table>



