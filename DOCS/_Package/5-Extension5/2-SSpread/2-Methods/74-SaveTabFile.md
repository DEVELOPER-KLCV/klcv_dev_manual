---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SaveTabFile Method
nav_order: 74
permalink: /package/extension5/sspread/methods/SaveTabFile
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SaveTabFile(<b>Writer</b>)</td>
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
    var f = fs.SaveDialog("Save", "Tab delimited file(*.txt)=*.txt", "", "");
    SaveTabFile(f);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exporttotextfile">ExportToTextFile</a>, <a href="/package/extension5/sspread/methods/loadtabfile">LoadTabFile</a>, <a href="/package/extension5/sspread/methods/loadtextfile">LoadTextFile</a>, <a href="/package/extension5/sspread/methods/savetabfileu">SaveTabFileU</a>, <a href="/package/extension5/sspread/methods/savetofile">SaveToFile</a> methods</td>
  </tr>
</table>
