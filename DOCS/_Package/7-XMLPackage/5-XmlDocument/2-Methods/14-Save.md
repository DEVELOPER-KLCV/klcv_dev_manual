---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.Save Method
nav_order: 14
permalink: /package/xmlpackage/xmldocument/methods/save
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">xmldoc.Save( <b>writer [, encoding</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Object <b>writer</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>encoding</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="4">Exception</td>
    <td>XML-4</td>
    <td></td>
  </tr>
  <tr>
    <td>XML-5</td>
    <td></td>
  </tr>
  <tr>
    <td>XML-18</td>
    <td></td>
  </tr>
  <tr>
    <td>XML-19</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var session = findHttpSession("http://host");
    var req = session.CreateRequest("path");
    xmldoc.Save(req);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



