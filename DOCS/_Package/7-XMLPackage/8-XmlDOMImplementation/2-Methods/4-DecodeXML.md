---
layout: default

grand_parent: XmlDOMImplementation Class
parent: Methods
has_children: false
title: XmlDOMImplementation.DecodeXML Method
nav_order: 4
permalink: /package/xmlpackage/xmldomimplementation/methods/decodexml
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = domimpl.DecodeXML( <b>str</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>str</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var enc = domimpl.EncodeXML("a >= 1 && b <= 1 || c == \"abc\"");
    print(enc, "\n");
    var dec = domimpl.DecodeXML(enc);
    print(dec, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmldomimplementation/methods/encodexml">EncodeXML</a> method</td>
  </tr>
</table>



