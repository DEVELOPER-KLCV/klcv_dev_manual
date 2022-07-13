---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportToExcelEx Method
nav_order: 23
permalink: /package/extension5/sspread/methods/exporttoexcelex
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify the sheet name and export to an Excel format file.<br><br>An extension of the ExportToExcel method. Method to handle the formulas can be specified.<br><small><span style="color:green">The following specifications have been expanded since Ver.5.0.2-></span></small><br>By specifying an existing Excel file, it is possible to export in the form of adding a sheet to the existing file. At that time, the existing file is not changed and is saved as a new Excel file with the sheet added. In addition, information other than sheets such as macros and graphs that exist in the existing Excel file will be deleted.</td>
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
    <td>Export destination <a href="/base/readerwriter#writer-object">Writer Object</a></td>
  </tr>
  <tr>
    <td><b>sheetname</b></td>
    <td>Sheet name to be created in the Excel file</td>
  </tr>
  <tr>
    <td><b>flags</b></td>
    <td>Set whether to export formulas<br>Specify the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-34fe{background-color:#c0c0c0;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-llyw{background-color:#c0c0c0;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-llyw">Constant</th>
    <th class="tg-34fe">Value</th>
    <th class="tg-llyw">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$SS_EXCELSAVEFLAGNONE</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">Save the formula</td>
  </tr>
  <tr>
    <td class="tg-0pky">$SS_EXCELSAVEFLAG_NOFORMULA</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">Do not save formulas</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td><b>URL or Reader</b></td>
    <td>The URL of the Excel file to read, or the <a href="/base/readerwriter#reader-object">ReaderObject</a><br>It can be omitted. If specified a URL, the file will be cached on your local computer for faster loading from the next time onwards. The latest file can always be obtained from the server by specifying the <a href="/package/httppackage/httpresponse">HttpResponse</a> object.<br><small><span style="color:red">Added since Ver.5.0.2</span></small></td>
  </tr>
  <tr>
    <td rowspan="4">Exception</td>
    <td>EXT-24</td>
    <td>No valid Reader object specified</td>
  </tr>
  <tr>
    <td>EXT-25</td>
    <td>No valid Writer object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the ExportToExcelEx method</td>
  </tr>
  <tr>
    <td>CRS-331</td>
    <td>Communication error<br>Same as the exception to the NetObject.Get method.</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportexcelbookex">ExportExcelBookEx</a>, <a href="/package/extension5/sspread/methods/exporttoexcel">ExportToExcel</a>, <a href="/package/extension5/sspread/methods/importexcelsheet">ImportExcelSheet</a> method</td><br><a href="/package/httppackage/httpresponse">HttpResponse</a> class
  </tr>
</table>
