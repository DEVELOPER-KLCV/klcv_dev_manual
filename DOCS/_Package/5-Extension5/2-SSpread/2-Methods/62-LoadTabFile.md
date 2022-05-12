---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.LoadTabFile Method
nav_order: 62
permalink: /package/extension5/sspread/methods/loadtabfile
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">LoadTabFile(<b>URL or Reader</b>)</td>
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
    var session = findHttpSession("http://example.com");
    var res = session.Get("tabfile.txt");
    LoadTextFile(res);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/loadfromfile">LoadFromFile</a>, <a href="/package/extension5/sspread/methods/loadtextfile">LoadTextFile</a>, <a href="/package/extension5/sspread/methods/savetabfile">SaveTabFile</a>, <a href="/package/extension5/sspread/methods/savetabfileu">SaveTabFileU</a> methods<br><a href="">HttpResponse</a> class</td>
  </tr>
</table>
