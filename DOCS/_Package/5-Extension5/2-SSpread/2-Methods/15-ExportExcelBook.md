---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportExcelBook Method
nav_order: 15
permalink: /package/extension5/sspread/methods/exportexcelbook
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportExcelBook(<b>Writer</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>Writer</b></td>
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
    var f = fs.SaveDialog("保存", "Excel File(*.xls)=*.xls", "xls", "");
    ExportExcelBook(f);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportexcelbookex">ExportExcelBookEx</a>, <a href="/package/extension5/sspread/methods/exporttoexcel">ExportToExcel</a>, <a href="/package/extension5/sspread/methods/importexcelsheet">ImportExcelSheet</a> methods</td>
  </tr>
</table>
