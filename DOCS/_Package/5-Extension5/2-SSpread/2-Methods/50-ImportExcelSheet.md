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
    <td colspan="2">Imports the specified sheet in an Excel file.<br><br>Files that can be imported are in Excel 2003 format (BIFF8 format).<br><br>The <a href="/package/extension5/sspread/methods/reset">Reset</a> method is called before importing and SSpread is initialized.<br><br>The number of sheets and sheet name of the Excel file to be imported can be checked with the <a href="/package/extension5/sspread/methods/getexcelsheetlist">GetExcelSheetList</a> method. In addition to specifying the sheet name in the argument <b>sheet</b>, a sheet number starting from 0 also can be specified.</td>
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
    <td>Excel file URL or <a href="/base/readerwriter#reader-object">Reader Object</a><br><br>The file will be cached on local computer for faster loading from the next time onwards when the URL is specified. The latest files from the server can be acquired by specifying an <a href="/package/httppackage/httpresponse">HttpResponse</a> object.</td>
  </tr>
  <tr>
    <td><b>sheet</b></td>
    <td>Sheet number or sheet name</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-24</td>
    <td>No valid Reader object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the ImportExcelSheet method</td>
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
