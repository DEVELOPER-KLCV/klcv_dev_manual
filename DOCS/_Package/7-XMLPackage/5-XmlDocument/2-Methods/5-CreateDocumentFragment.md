---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.CreateDocumentFragment Method
nav_order: 5
permalink: /package/xmlpackage/xmldocument/methods/createdocumentfragment
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Create a DocumentFragment node.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var df = xmldoc.CreateDocumentFragment( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlDocumentFragment object</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
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
    var xmldoc = domImpl.Load(res);
    var df = xmldoc.CreateDocumentFragment();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmldocumentfragment">XmlDocumentFragment</a> class</td>
  </tr>
</table>



