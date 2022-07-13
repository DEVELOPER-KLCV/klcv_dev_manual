---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportToHTMLEx Method
nav_order: 25
permalink: /package/extension5/sspread/methods/exporttohtmlex
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Export all cells to an HTML file. An extension of the  <a href="/package/extension5/sspread/methods/exporttohtml">ExportToHTML</a>  method.<br><br> The style information can be specified to be output to the HTML table. <br><br>Use the <a href="/package/extension5/sspread/methods/exportrangetohtmlex">ExportRangeToHTMLEx</a> method to export a specific cell range.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportToHTMLEx(<b>Writer</b>, <b>title</b>, <b>css</b>, <b>table</b>, <b>tr</b>, <b>td</b>, <b>th</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="7">Arguments</td>
    <td><b>Writer</b></td>
    <td>Export destination <a href="/base/readerwriter#writer-object">Writer Object</a></td>
  </tr>
  <tr>
    <td><b>title</b></td>
    <td>HTML page title</td>
  </tr>
  <tr>
    <td><b>css</b></td>
    <td>CSS file name</td>
  </tr>
  <tr>
    <td><b>table</b></td>
    <td>Table tag class name</td>
  </tr>
  <tr>
    <td><b>tr</b></td>
    <td>Tr tag class name</td>
  </tr>
  <tr>
    <td><b>td</b></td>
    <td>Td tag class name</td>
  </tr>
  <tr>
    <td><b>th</b></td>
    <td>Th tag class name</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-25</td>
    <td>No valid Writer object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the ExportToHTMLEx method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.SaveDialog("Save", "HTML File(*.html)=*.html", "html", "");
    ExportToHTMLEx(f, "XX Table", "http://example.com/sample.css", "ctable", "ctr", "ctd", "cth");
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportrangetohtml">ExportRangeToHTML</a>, <a href="/package/extension5/sspread/methods/exportrangetohtmlex">ExportRangeToHTMLEx</a>, <a href="/package/extension5/sspread/methods/exporttohtml">ExportToHTML</a> method</td>
  </tr>
</table>
