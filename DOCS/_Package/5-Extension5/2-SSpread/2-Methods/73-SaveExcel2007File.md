---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SaveExcel2007File Method
nav_order: 73
permalink: /package/extension5/sspread/methods/saveexcel2007file
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SaveExcel2007File(<b>Writer</b>, <b>password</b>, <b>flags[, sheetname[, URL or Reader]]</b>)</td>
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
    <td><b>password</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>flags</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>sheetname</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>URL or Reader</b></td>
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
    var f = fs.SaveDialog("Save", "Excel2007 File(*.xlsx)=*.xlsx", "xlsx", "");
    SaveExcel2007File(f, "Biz", $SS_EXCELSAVEFLAG_NOFORMULAS, "Sheet 1");
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/isexcel2007file">IsExcel2007File</a>, <a href="/package/extension5/sspread/methods/openexcel2007file">OpenExcel2007File</a> methods<br><a href="/package/httppackage/httpresponse">HttpResponse</a> class</td>
  </tr>
</table>
