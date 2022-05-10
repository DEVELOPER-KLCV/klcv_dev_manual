---
layout: default

grand_parent: XmlDOMImplementation Class
parent: Methods
has_children: false
title: XmlDOMImplementation.Load Method
nav_order: 7
permalink: /package/xmlpackage/xmldomimplementation/methods/load
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var xmldoc = domimpl.Load( <b>reader</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Object <b>reader</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="4">Exception</td>
    <td>XML-1</td>
    <td></td>
  </tr>
  <tr>
    <td>XML-2</td>
    <td></td>
  </tr>
  <tr>
    <td>XML-3</td>
    <td></td>
  </tr>
  <tr>
    <td>XML-13</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmldocument">XmlDocument</a> class<br><a href="/package/xmlpackage/xmldomimplementation/methods/parse">Parse</a> method</td>
  </tr>
</table>



