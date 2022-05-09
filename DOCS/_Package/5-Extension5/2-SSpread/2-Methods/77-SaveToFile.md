---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SaveToFile Method
nav_order: 77
permalink: /package/extension5/sspread/methods/SaveToFile
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SaveToFile(<b>Writer</b>, <b>dataonly</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>Writer</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>dataonly</b></td>
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
    var f = fs.SaveDialog("Save", "SSpread saved data(*.*)=*.*", "", "");
    SaveToFile(f, $FALSE);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exporttotextfile">ExportToTextFile</a>, <a href="/package/extension5/sspread/methods/loadfromfile">LoadFromFile</a><a href="/package/extension5/sspread/methods/SaveTabFile">SaveTabFile</a> methods</td>
  </tr>
</table>
