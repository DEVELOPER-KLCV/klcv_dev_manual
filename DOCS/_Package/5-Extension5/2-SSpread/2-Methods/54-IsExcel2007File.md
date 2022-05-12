---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.IsExcel2007File Method
nav_order: 54
permalink: /package/extension5/sspread/methods/isexcel2007file
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">IsExcel2007File(<b>URL or Reader</b>)</td>
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
    <td>Exception</td>
    <td>EXT-24</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var session = findHttpSession("http://example.com");
    var res = session.Get("excel2007file.xlsx");
    if (IsExcel2007File(res) > 0) {
        MessageBox("This is an Excel 2007 format file");
    }
    </pre></code></td>
  </tr>
   <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/openexcel2007file">OpenExcel2007File</a>, <a href="/package/extension5/sspread/methods/saveexcel2007file">SaveExcel2007File</a> methods<br><a href="/package/httppackage/httpresponse">HttpResponse</a> class</td>
  </tr>
</table>
