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
    <td colspan="2">Read XML from the Reader object .<br>It is used when loading an XML file from a web server or file .</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var xmldoc = domimpl.Load( <b>reader</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlDocument object</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Object <b>reader</b></td>
    <td><a href="/base/readerwriter#reader-object">ReaderObject</a> to read from (object that can use ReadLine method)</td>
  </tr>
  <tr>
    <td rowspan="4">Exception</td>
    <td>XML-1</td>
    <td>XML parse error</td>
  </tr>
  <tr>
    <td>XML-2</td>
    <td>No valid Read object specified</td>
  </tr>
  <tr>
    <td>XML-3</td>
    <td>Does not support the ReadLine () method</td>
  </tr>
  <tr>
    <td>XML-13</td>
    <td>Input XML is empty</td>
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



