---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.CreateProcessingInstruction Method
nav_order: 8
permalink: /package/xmlpackage/xmldocument/methods/createprocessinginstruction
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var pi = xmldoc.CreateProcessingInstruction( <b>target, data</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>target</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>data</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>DOM-5</td>
    <td>INVALID_CHARACTER_ERR</td>
  </tr><tr>
    <td>DOM-9</td>
    <td>NOT_SUPPORTED_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var pi = xmldoc.CreateProcessingInstruction("xml", "version=\"1.0\"");
    xmldoc.AppendChild(pi);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlprocessinginstruction">XmlProcessingInstruction</a> class</td>
  </tr>
</table>



