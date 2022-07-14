---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.IsExcel2007File Method
nav_order: 54
permalink: /package/extension5/sspread/methods/isexcel2007file
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Find out if the file is an Excel 2007 format workbook and if it is protected<br><small><span style="color:red">Added since Ver.5.0.2</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">IsExcel2007File(<b>URL or Reader</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">The following values are returned<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-z50u">Value</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Not an Excel 2007 format file</td>
  </tr>
  <tr>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Excel 2007 format file</td>
  </tr>
  <tr>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Password protected Excel 2007 format file</td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>URL or Reader</b></td>
    <td>The URL of the Excel2007 format file to be read , or the <a href="/base/readerwriter#reader-object">Reader Object</a><br><br> The file will be cached on local computer for faster loading from the next time onwards if URL is specified. The latest files from the server can be acquired by specifying an HttpResponse object.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-24</td>
    <td>No valid Reader object specified</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var session = findHttpSession("http://example.com");
    var res = session.Get("excel2007file.xlsx");
    if (IsExcel2007File(res) > 0) {
        MessageBox("This is an Excel 2007 format file");
    }
    </pre></code></td>
  </tr>
   <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/openexcel2007file">OpenExcel2007File</a>, <a href="/package/extension5/sspread/methods/saveexcel2007file">SaveExcel2007File</a> methods<br><a href="/package/httppackage/httpresponse">HttpResponse</a> class</td>
  </tr>
</table>
