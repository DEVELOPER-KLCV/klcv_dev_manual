---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportToHTML Method
nav_order: 24
permalink: /package/extension5/sspread/methods/ExportToHTML
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
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
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-25</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td></td>
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
