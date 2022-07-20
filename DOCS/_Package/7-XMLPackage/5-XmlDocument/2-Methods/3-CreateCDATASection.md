---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.CreateCDATASection Method
nav_order: 3
permalink: /package/xmlpackage/xmldocument/methods/CreateCDATASection
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Create a CDATASection node.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var cd = xmldoc.CreateCDATASection( <b>data</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlCDATASection object</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>data</b></td>
    <td>A string that is the initial value of the CDATASection node</td>
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
    var cd = xmldoc.CreateCDATASectione("ABC");
    xmldoc.DocumentElement.AppendChild(cd);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlcdatasection">XmlCDATASection</a> class</td>
  </tr>
</table>



