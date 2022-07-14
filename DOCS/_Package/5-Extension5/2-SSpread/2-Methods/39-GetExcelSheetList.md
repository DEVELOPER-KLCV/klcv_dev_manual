---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetExcelSheetList Method
nav_order: 39
permalink: /package/extension5/sspread/methods/getexcelsheetlist
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the sheet name list from the specified Excel file.<br>The acquired sheet name can be used to specify the sheet name of the <a href="/package/extension5/sspread/methods/importexcelsheet">ImportExcelSheet</a> method.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetExcelSheetList(<b>URL or Reader</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">UString array object containing a list of sheet names</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>URL or Reader</b></td>
    <td>Excel file URL or <a href="/base/readerwriter#reader-object">Reader Object</a><br><br>If specify a URL, the file will be cached on local computer for faster loading from the next time onwards. The latest files from the server can be acquired by specifying an <a href="/package/httppackage/httpresponse">HttpResponse</a> object.</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-24</td>
    <td>No valid Reader object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the GetExcelSheetList method</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportexcelbook">ExportExcelBook</a>, <a href="/package/extension5/sspread/methods/exportexcelbookex">ExportExcelBookEx</a>, <a href="/package/extension5/sspread/methods/exporttoexcel">ExportToExcel</a>, <a href="/package/extension5/sspread/methods/exporttoexcelex">ExportToExcelEx</a>, <a href="/package/extension5/sspread/methods/importexcelsheet">ImportExcelSheet</a> methods<br><a href="/package/httppackage/httpresponse">HttpResponse</a> class</td>
  </tr>
</table>
