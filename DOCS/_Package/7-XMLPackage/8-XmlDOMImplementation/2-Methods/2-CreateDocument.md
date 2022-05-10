---
layout: default

grand_parent: XmlDOMImplementation Class
parent: Methods
has_children: false
title: XmlDOMImplementation.CreateDocument Method
nav_order: 2
permalink: /package/xmlpackage/xmldomimplementation/methods/createdocument
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var xmldoc = domimpl.CreateDocument( <b>namespaceURI, qualifiedName, doctype</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>String <b>namespaceURI</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>qualifiedName</b></td>
    <td></td>
  </tr>
  <tr>
    <td>XmlDocumentType <b>doctype</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>DOM-5</td>
    <td>INVALID_CHARACTER_ERR</td>
  </tr>
  <tr>
    <td>DOM-14</td>
    <td>NAMESPACE_ERR</td>
  </tr>
  <tr>
    <td>DOM-4</td>
    <td>WRONG_DOCUMENT_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var domimpl = new XmlDOMImplementation;
    var xmldoc = domimpl.CreateDocument("http://www.w3.org/2000/svg", "svg", null);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmldocument">XmlDocument</a> class<br><a href="/package/xmlpackage/xmldomimplementation/methods/createdocumenttype">CreateDocumentType</a> method</td>
  </tr>
</table>



