---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportToHTML Method
nav_order: 24
permalink: /package/extension5/sspread/methods/exporttohtml
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Export all cells to an HTML file. <br><br>In the destination HTML file, the spreadsheet cells are displayed as an HTML table. <br><br>Use the <a href="/package/extension5/sspread/methods/exportrangetohtmlex">ExportRangeToHTMLEx</a> method to export a specific cell range. <br><br>Use the <a href="/package/extension5/sspread/methods/exporttohtmlex">ExportToHTMLEx</a>  method to specify style information.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportToHTML(<b>Writer</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>Writer</b></td>
    <td>Export destination <a href="/base/readerwriter#writer-object">Writer Object</a></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-25</td>
    <td>No valid Writer object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the ExportToHTML method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.SaveDialog("Save", "HTML File(*.html)=*.html", "html", "");
    ExportToHTML(f);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportrangetohtml">ExportRangeToHTML</a>, <a href="/package/extension5/sspread/methods/exportrangetohtmlex">ExportRangeToHTMLEx</a>, <a href="/package/extension5/sspread/methods/exporttohtmlex">ExportToHTMLEx</a> method</td>
  </tr>
</table>
