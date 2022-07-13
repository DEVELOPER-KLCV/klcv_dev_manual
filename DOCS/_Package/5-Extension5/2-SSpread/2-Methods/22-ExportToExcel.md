---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportToExcel Method
nav_order: 22
permalink: /package/extension5/sspread/methods/exporttoxcel
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify the sheet name and export to an Excel format file.<br><br> The exported file will be in the format up to Excel 2003 (BIFF8 format). <br><br>If you want to specify how to handle the formula, use the <a href="/package/extension5/sspread/methods/exporttoexcelex">ExportToExcelEx</a> method tp specify].</td>
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
    <td>Export destination <a href="/base/readerwriter#writer-object">Writer Object</a></td>
  </tr>
  <tr>
    <td><b>sheetname</b></td>
    <td>Sheet name to be created in the Excel file</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-25</td>
    <td>No valid Writer object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>	An error occurred in the ExportToExcel method</td>
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
