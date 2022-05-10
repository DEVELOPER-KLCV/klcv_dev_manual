---
layout: default

grand_parent: XmlDOMImplementation Class
parent: Methods
has_children: false
title: XmlDOMImplementation.Parse Method
nav_order: 8
permalink: /package/xmlpackage/xmldomimplementation/methods/parse
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var xmldoc = domimpl.Parse( <b>xmltext</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>xmltext</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>XML-1</td>
    <td></td>
  </tr>
  <tr>
    <td>XML-13</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var src = "&lt;?xml version=\"1.0\" … ";
    var domimpl = new XmlDOMImplementation;
    var xmldoc = domimpl.Parse(src);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmldocument">XmlDocument</a> class<br><a href="/package/xmlpackage/xmldomimplementation/methods/load">Load</a> method</td>
  </tr>
</table>



