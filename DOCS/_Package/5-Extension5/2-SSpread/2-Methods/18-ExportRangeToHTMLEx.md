---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportRangeToHTMLEx Method
nav_order: 18
permalink: /package/extension5/sspread/methods/exportrangetohtmlex
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportRangeToHTMLEx(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>, <b>Writer</b>, <b>title</b>, <b>css</b>, <b>table</b>, <b>tr</b>, <b>td</b>, <b>th</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="11">Arguments</td>
    <td><b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>Writer</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>title</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>css</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>table</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>tr</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>td</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>th</b></td>
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
    var f = fs.SaveDialog("Save", "HTMLFile(*.html)=*.html", "html", "");
    ExportRangeToHTMLEx(1, 1, 10, 10, f, "XX Table", "http://example.com/sample.css", "ctable", "ctr", "ctd", "cth");
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportrangetohtml">ExportRangeToHTML</a>, <a href="/package/extension5/sspread/methods/exporttohtml">ExportToHTML</a>, <a href="/package/extension5/sspread/methods/exporttohtmlex">ExportToHTMLEx</a> methods</td>
  </tr>
</table>
