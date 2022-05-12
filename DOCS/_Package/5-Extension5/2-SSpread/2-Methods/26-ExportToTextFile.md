---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportToTextFile Method
nav_order: 26
permalink: /package/extension5/sspread/methods/exporttotextfile
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportToTextFile(<b>Writer</b>, <b>celldelim</b>, <b>coldelim</b>, <b>rowdelim</b>, <b>flags</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="5">Arguments</td>
    <td><b>Writer</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>celldelim</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>coldelim</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>rowdelim</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>flags</b></td>
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
    ExportToHTMLEx(f, "XX Table", "http://example.com/sample.css", "ctable", "ctr", "ctd", "cth");
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportrangetotextfile">ExportRangeToTextFile</a>, <a href="/package/extension5/sspread/methods/exporttotextfileu">ExportToTextFileU</a>, <a href="/package/extension5/sspread/methods/loadtextfile">LoadTextFile</a> method</td>
  </tr>
</table>
