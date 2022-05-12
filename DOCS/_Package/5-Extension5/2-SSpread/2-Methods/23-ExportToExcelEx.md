---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportToExcelEx Method
nav_order: 23
permalink: /package/extension5/sspread/methods/exporttoex
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportToExcelEx(<b>Writer</b>, <b>sheetname</b>, <b>[, URL or reader]</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td><b>Writer</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>sheetname</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>flags</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>URL or Reader</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="4">Exception</td>
    <td>EXT-24</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-25</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td></td>
  </tr>
  <tr>
    <td>CRS-331</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.SaveDialog("Save", "Excel File(*.xls)=*.xls", "xls", "");
    ExportToExcelEx(f, "Sheet 1", $SS_EXCELSAVEFLAG_NOFORMULAS);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportexcelbookex">ExportExcelBookEx</a>, <a href="/package/extension5/sspread/methods/exporttoexcel">ExportToExcel</a>, <a href="/package/extension5/sspread/methods/importexcelsheet">ImportExcelSheet</a> method</td><br><a href="">HttpResponse</a> class
  </tr>
</table>
