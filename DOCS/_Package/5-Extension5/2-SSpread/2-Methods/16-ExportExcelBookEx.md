---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportExcelBookEx Method
nav_order: 16
permalink: /package/extension5/sspread/methods/exportexcelbookex
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Export to an Excel format file.<br><br>An extension of the ExportExcelBook method. How to handle formulas can be specified.<br><br>Use the ExportToExcelEx method to specify the sheet name.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportExcelBookEx(<b>Writer</b>, <b>flags</b>)</td>
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
    <td><b>flags</b></td>
    <td>Set whether to export formulas<br> Specify the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-266k{background-color:#9b9b9b;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-9u2q{background-color:#9b9b9b;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-266k">Constant</th>
    <th class="tg-9u2q">Value</th>
    <th class="tg-266k">Description</th>
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
    <td rowspan="2">Exception</td>
    <td>EXT-25</td>
    <td>No valid Writer object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the ExportExcelBookEx method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.SaveDialog("Save", "Excel File(*.xls)=*.xls", "xls", "");
    ExportExcelBookEx(f, $SS_EXCELSAVEFLAG_NOFORMULAS);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportexcelbook">ExportExcelBook</a>, <a href="/package/extension5/sspread/methods/exporttoexcelex">ExportToExcelEx</a>, <a href="/package/extension5/sspread/methods/importexcelsheet">ImportExcelSheet</a> methods</td>
  </tr>
</table>
