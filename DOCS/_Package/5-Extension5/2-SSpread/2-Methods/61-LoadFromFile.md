---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.LoadFromBuffer Method
nav_order: 61
permalink: /package/extension5/sspread/methods/LoadFromFile
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">LoadFromFile(<b>URL or Reader</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>URL or Reader</b></td>
    <td></td>
  </tr>  
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-24</td>
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
    var f = fs.OpenDialog("Open", "SSpread Save Data(*.*)=*.*", "", "");
    LoadFromFile(f);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/loadtabfile">LoadTabFile</a>, <a href="/package/extension5/sspread/methods/loadtextfile">LoadTextFile</a>, <a href="/package/extension5/sspread/methods/savetofile">SaveToFile</a> methods<br><a href="">HttpResponse</a> class</td>
  </tr>
</table>
