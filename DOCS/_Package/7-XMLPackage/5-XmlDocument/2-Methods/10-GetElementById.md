---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.GetElementById Method
nav_order: 10
permalink: /package/xmlpackage/xmldocument/methods/getelementbyid
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Search for the Element node from the ID attribute.<br><br>The name of the ID attribute to be searched can be changed with the <a href="/package/xmlpackage/xmldocument/properties/IndexAttributeName">IndexAttributeName</a> property.When the IndexAttributeName property is not set, the attribute named "ID" (case sensitive) is searched as the ID attribute.<br><br><small><span style="color:red">Added since Ver.4.0.0</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var elm = xmldoc.GetElementById( <b>elementId</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlElement object with the specified ID attribute.<br>If not found, null is returned.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>elementId</b></td>
    <td>The value specified for the ID attribute to be searched</td>
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
    xmldoc.IndexAttributeName = "id";
    var elm = xmldoc.GetElementById("1001");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlelement">XmlElement</a> class<br><a href="/package/xmlpackage/xmldocument/properties/IndexAttributeName">IndexAttributeName</a> property<br><a href="/package/xmlpackage/xmldocument/methods/GetElementsByTagName">GetElementsByTagName</a>, <a href="/package/xmlpackage/xmldocument/methods/GetElementsByTagNameNS">GetElementsByTagNameNS</a> methods</td>
  </tr>
</table>



