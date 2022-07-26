---
layout: default

grand_parent: XmlElement Class
parent: Methods
has_children: false
title: XmlElement.GetElementsByTagNameNS Method
nav_order: 6
permalink: /package/xmlpackage/xmlelement/methods/getelementsbytagnamens
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Search for Element nodes by namespace URI and tag name to get a list of matching Element nodes.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var list = elm.GetElementByTagNameNS( <b>namespaceURI, tagName</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlNodeList object containing Element nodes that match the criteria

If not found, it returns an empty XmlNodeList object.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>namespaceURI</b></td>
    <td>Namespace URI to search</td>
  </tr>
  <tr>
    <td>String <b>tagName</b></td>
    <td>Tag name to search</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var elm = xmldoc.DocumentElement;
    var list = elm.GetElementByTagNameNS("http://www.w3.org/2000/svg", "rect");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnodelist">XmlNodeList</a>, <a href="/package/xmlpackage/xmlelement">XmlElement</a> class<br><a href="/package/xmlpackage/xmlelement/methods/getelementsbytagname">GetElementsByTagName</a> method</td>
  </tr>
</table>



