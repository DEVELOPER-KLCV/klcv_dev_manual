---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.CreateComment Method
nav_order: 4
permalink: /package/xmlpackage/xmldocument/methods/createcomment
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Create a Comment node.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var comment = xmldoc.CreateComment( <b>data</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlComment object</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>data</b></td>
    <td>Character string that be the initial value of the Comment node</td>
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
    var comment = xmldoc.CreateComment("ABC");
    xmldoc.DocumentElement.AppendChild(comment);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlcomment">XmlComment</a> class</td>
  </tr>
</table>



