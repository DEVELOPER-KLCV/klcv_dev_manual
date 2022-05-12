---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.OpenExcel2007File Method
nav_order: 67
permalink: /package/extension5/sspread/methods/openexcel2007file
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">OpenExcel2007File(<b>URL or Reader</b>, <b>password</b>, <b>reserved</b>, <b>excelSheet</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td><b>URL or Reader</b></td>
    <td></td>
  </tr>  
  <tr>
    <td><b>password</b></td>
    <td></td>
  </tr>  
  <tr>
    <td><b>reserved</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>sheet</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>EXT-1</td>
    <td></td>
  </tr>
  <tr>
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
    var res = session.Get("/excelfile.xlsx");
    OpenExcel2007File(res, "Biz", 0, 0);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/isexcel2007file">IsExcel2007File</a>, <a href="/package/extension5/sspread/methods/saveexcel2007file">SaveExcel2007File</a> methods<br><a href="/package/httppackage/httpresponse">HttpResponse</a> class</td>
  </tr>
</table>
