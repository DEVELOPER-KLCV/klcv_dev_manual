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
    <td colspan="2">Imports the specified sheet in an Excel file.<br><br>Files that can be imported are in Excel 2007 or later format (xlsx).<br><br>The <a href="/package/extension5/sspread/methods/reset">Reset</a> method is called before importing and SSpread is initialized.<br><br>The format of the Excel file to be imported can be checked with the <a href="/package/extension5/sspread/methods/isexcel2007file">IsExcel2007File</a> method and the password protection status.<br><small><span style="color:red">Added since Ver.5.0.2</span></small></td>
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
    <td>Excel2007 format file URL or <a href="/base/readerwriter#reader-object">Reader Object</a><br><br> If a URL is specified, the file will be cached on local computer for faster loading from the next time onwards.The latest files from the server by specifying an HttpResponse object. The latest files from the server can always acquired by specifying an <a href="/package/httppackage/httpresponse">HttpResponse</a> object.</td>
  </tr>  
  <tr>
    <td><b>password</b></td>
    <td>Workbook password. Null or "" (empty string) if not needed</td>
  </tr>  
  <tr>
    <td><b>reserved</b></td>
    <td>Specify 0</td>
  </tr>
  <tr>
    <td><b>sheet</b></td>
    <td>Sheet number starting from 0</td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>EXT-1</td>
    <td>The argument of OpenExcel2007File is invalid.</td>
  </tr>
  <tr>
    <td>EXT-24</td>
    <td>No valid Reader object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the OpenExcel2007File method</td>
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
