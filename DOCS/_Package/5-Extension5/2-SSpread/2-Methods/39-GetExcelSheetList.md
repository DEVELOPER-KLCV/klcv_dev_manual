---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetExcelSheetList Method
nav_order: 39
permalink: /package/extension5/sspread/methods/GetExcelSheetList
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetExcelSheetList(<b>URL or Reader</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>col</b></td>
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
    var res = session.Get("/excelfile.xls");
    var ret = GetExcelSheetList(res);
    
    print("Sheet Count", ret.Length, "\n");
    for (var i = 0; i < ret.Length; i++) {
        print(ret[i], "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/ExportExcelBook">ExportExcelBook</a>, <a href="/package/extension5/sspread/methods/ExportExcelBookEx">ExportExcelBookEx</a>, <a href="/package/extension5/sspread/methods/ExportToExcel">ExportToExcel</a>, <a href="/package/extension5/sspread/methods/ExportToExcelEx">ExportToExcelEx</a>, <a href="/package/extension5/sspread/methods/ImportExcelSheet">ImportExcelSheet</a> methods<br><a href="">HttpResponse</a> class</td>
  </tr>
</table>
