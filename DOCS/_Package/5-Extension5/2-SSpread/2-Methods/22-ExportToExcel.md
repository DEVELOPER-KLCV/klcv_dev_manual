---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportToExcel Method
nav_order: 22
permalink: /package/extension5/sspread/methods/ExportToExcel
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportToExcel(<b>Writer</b>, <b>sheetname</b>)</td>
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
    <td><b>sheetname</b></td>
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
    var f = fs.SaveDialog("Save", "Excel File(*.xls)=*.xls", "xls", "");
    ExportToExcel(f, "Sheet 1");
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportexcelbook">ExportExcelBook</a>, <a href="/package/extension5/sspread/methods/exporttoexcelex">ExportToExcelEx</a>, <a href="/package/extension5/sspread/methods/importexcelsheet">ImportExcelSheet</a> method</td>
  </tr>
</table>
