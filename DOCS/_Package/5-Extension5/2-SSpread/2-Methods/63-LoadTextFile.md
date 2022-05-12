---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.LoadTextFile Method
nav_order: 63
permalink: /package/extension5/sspread/methods/loadtextfile
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">LoadTextFile(<b>URL or Reader</b>, <b>celldelim</b>, <b>coldelim</b>, <b>rowdelim</b>, <b>flags</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="5">Arguments</td>
    <td><b>URL or Reader</b></td>
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
    var res = session.Get("textfile.txt");
    LoadTextFile(res, "", ",", "", $LoadTextFileNoHeaders);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportrangetotextfile">ExportRangeToTextFile</a>, <a href="/package/extension5/sspread/methods/exporttotextfile">ExportToTextFile</a>, <a href="/package/extension5/sspread/methods/loadfromfile">LoadFromFile</a>, <a href="/package/extension5/sspread/methods/loadtabfile">LoadTabFile</a> methods<br><a href="/package/httppackage/httpresponse">HttpResponse</a> class</td>
  </tr>
</table>
