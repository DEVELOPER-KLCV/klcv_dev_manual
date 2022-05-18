---
layout: default

grand_parent: Doc Class
parent: Methods
has_children: false
title: Doc.GetPageReader Method
nav_order: 2
permalink: /package/standard/doc/methods/getpagereader
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns a File object that opens an SVG file on the specified page in read mode.<br><small><span style="color:red">Added since Ver.4.0.5</span></small><br>The returned File object can be passed as XML to the <a href="/package/xmlpackage/xmldomimplementation/methods/load">Load</a> method of the <a href="/package/xmlpackage/xmldomimplementation">XmlDOMImplementation</a> class. It is also possible to specify the generated <a href="/package//xmlpackage/xmldocument">XMLDocument</a> object in the <a href="/package/standard/form/properties/bgpattern">BgPattern</a> property of the <a href="/package/standard/form/">Form</a> class and display it as an SVG image.<br><br>Unlike the <a href="/package/standard/doc/methods/getpagefile">GetPageFile</a> method, the GetPageReader method returns an SVG in a File object, so it can handle links to image files correctly.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var svgfile = Doc1.GetPageReader( <b>page</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">File object that opened the SVG file of the target page</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>page</b></td>
    <td>Page number you want to get</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>RTM-3</td>
    <td>Could not open the file</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
Doc1.Preview = $FILE;
Doc1.ShowPage();
var svgfile = Doc1.GetPageReader(1);
Doc1.Delete();
var impl = new XmlDOMImplementation;
var xmldoc = impl.Load(svgfile);
svgfile.Close();
Form1.BgPattern = xmldoc;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/doc/methods/getpagefile">GetPageFile</a> method</td>
  </tr>
</table>