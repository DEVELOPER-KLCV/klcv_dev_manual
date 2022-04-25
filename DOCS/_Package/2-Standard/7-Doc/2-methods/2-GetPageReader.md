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
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var svgfile = Doc1.GetPageReader( <b>page</b> )</td>
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
    <td>RTM-3</td>
    <td></td>
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
    <td colspan="2"><a href="/package/standard/doc/methods/GetPageFile">GetPageFile</a> method</td>
  </tr>
</table>