---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ImportExcelSheet Method
nav_order: 50
permalink: /package/extension5/sspread/methods/importexcelsheet
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ImportExcelSheet(<b>URL or Reader</b>, <b>sheet</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>URL or Reader</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>sheet</b></td>
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
    ImportExcelSheet(res, "Sheet 1");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportexcelbook">ExportExcelBook</a>, <a href="/package/extension5/sspread/methods/exportexcelbookex">ExportExcelBookEx</a>, <a href="/package/extension5/sspread/methods/exporttoexcel">ExportToExcel</a>, <a href="/package/extension5/sspread/methods/exporttoexcelex">ExportToExcelEx</a>, <a href="/package/extension5/sspread/methods/getexcelsheetlist">GetExcelSheetList</a> methods<br><a href="/package/httppackage/httpresponse">HttpResponse</a> class</td>
  </tr>
</table>
