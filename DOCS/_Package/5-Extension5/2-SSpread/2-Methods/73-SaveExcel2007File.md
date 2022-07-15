---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SaveExcel2007File Method
nav_order: 73
permalink: /package/extension5/sspread/methods/saveexcel2007file
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify the sheet name and export it to an Excel 2007 format file. Method to handle the formulas can be specified.<br><br> By specifying an existing Excel 2007 format file, it is possible to export by adding a sheet to the existing file. At that time, the existing file is not changed and is saved as a new Excel file with the sheet added. In addition, information other than sheets such as macros and graphs that exist in the existing Excel file will be deleted.<br><br> <span style="color:red">Notes on use</span><br>The Excel file output by this method is not a complete guarantee of compatibility with sheets created in Excel. Also, for better compatibility, it is recommended to save in Excel 2003 format. <br><br><small><span style="color:red">Added since Ver.5.0.2</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SaveExcel2007File(<b>Writer</b>, <b>password</b>, <b>flags[, sheetname[, URL or Reader]]</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="5">Arguments</td>
    <td><b>Writer</b></td>
    <td>Export to <a href="/base/readerwriter#writer-object">Writer Object</a></td>
  </tr>
  <tr>
    <td><b>password</b></td>
    <td>Workbook protection password. Null or "" (empty string) if not needed</td>
  </tr>
  <tr>
    <td><b>flags</b></td>
    <td>Set whether to export formulas<br>Specify the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-z50u">Value</th>
    <th class="tg-xt05">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$SS_EXCELSAVEFLAGNONE</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Save the formula</td>
  </tr>
  <tr>
    <td class="tg-0lax">$SS_EXCELSAVEFLAG_NOFORMULAS</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Do not save formulas</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td><b>sheetname</b></td>
    <td>Sheet name to be created in the Excel file. Optional.</td>
  </tr>
  <tr>
    <td><b>URL or Reader</b></td>
    <td>URL of Excel 2007 format file to read, or <a href="/base/readerwriter#reader-object">Reader Object</a><br><br> The file will be cached on local computer for faster loading from the next time onwards if URL is specified. The latest files can be acquired from the server by specifying an <a href="/package/httppackage/httpresponse">HttpResponse</a> object.</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-25</td>
    <td>No valid Writer object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the SaveExcel2007File method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.SaveDialog("Save", "Excel2007 File(*.xlsx)=*.xlsx", "xlsx", "");
    SaveExcel2007File(f, "Biz", $SS_EXCELSAVEFLAG_NOFORMULAS, "Sheet 1");
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/isexcel2007file">IsExcel2007File</a>, <a href="/package/extension5/sspread/methods/openexcel2007file">OpenExcel2007File</a> methods<br><a href="/package/httppackage/httpresponse">HttpResponse</a> class</td>
  </tr>
</table>
