---
layout: default

grand_parent: Doc Class
parent: Methods
has_children: false
title: Doc.GetPageFile Method
nav_order: 1
permalink: /package/standard/doc/methods/getpagefile
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the SVG of the specified page as a string.<br><br>The returned SVG string can be passed to the <a href="/package/xmlpackage/xmldomimplementation/methods/parse">Parse</a> method of the <a href="/package/xmlpackage/xmldomimplementation">XmlDOMImplementation</a> class and manipulated as XML. It is also possible to specify the generated <a href="/package//xmlpackage/xmldocument">XMLDocument</a> object in the <a href="/package/standard/form/properties/bgpattern">BgPattern</a> property of the <a href="/package/standard/form/">Form</a> class and display it as an SVG image.<br><br>Use the <a href="/package/standard/doc/methods/getpagereader">GetPageReader</a> method when dealing with pages containing images. The GetPageReader method can handle links to image files correctly.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var svgtext = Doc1.GetPageFile( <b>page</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">SVG string on the specified page</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>page</b></td>
    <td>Page number you want to get</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>PKG-7</td>
    <td>The specified page file cannot be found</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
Doc1.Preview = $FILE;
Doc1.ShowPage();
var svgtext = Doc1.GetPageFile(1);
Doc1.Delete();
var impl = new XmlDOMImplementation;
var xmldoc = impl.Parse(svgtext);
Form1.BgPattern = xmldoc;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/doc/methods/getpagereader">GetPageReader</a> method</td>
  </tr>
</table>