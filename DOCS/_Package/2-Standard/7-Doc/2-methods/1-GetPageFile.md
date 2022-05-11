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
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var svgtext = Doc1.GetPageFile( <b>page</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>page</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>PKG-7</td>
    <td></td>
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