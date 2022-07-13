---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportToTextFileU Method
nav_order: 27
permalink: /package/extension5/sspread/methods/exporttotextfileu
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Export the spreadsheet to a Unicode text file using your own specified delimiter.<br><br> It has the same function as the ExportToTextFile method, but the output result is a Unicode text file. <br><br>Use the ExportRangeToTextFileU method to export a specific cell range.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportToTextFileU(<b>Writer</b>, <b>celldelim</b>, <b>coldelim</b>, <b>rowdelim</b>, <b>flags</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="5">Arguments</td>
    <td><b>Writer</b></td>
    <td>Export destination <a href="/base/readerwriter#writer-object">Writer Object</a></td>
  </tr>
  <tr>
    <td><b>celldelim</b></td>
    <td>Character string representing the cell delimiter</td>
  </tr>
  <tr>
    <td><b>coldelim</b></td>
    <td>A string representing the column delimiter</td>
  </tr>
  <tr>
    <td><b>rowdelim</b></td>
    <td>A string representing the line delimiter</td>
  </tr>
  <tr>
    <td><b>flags</b></td>
    <td>Method to create a file<br>Specify a combination of the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-tcrt{font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-i7zr{font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Constant</th>
    <th class="tg-cqgq">Value</th>
    <th class="tg-0ss8">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">$ExportToTextFileUnformattedData</td>
    <td class="tg-lcf4">4</td>
    <td class="tg-j5n6">Export as unformatted data</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ExportToTextFileColHeaders</td>
    <td class="tg-lcf4">8</td>
    <td class="tg-j5n6">Export column header string</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$ExportToTextFileRowHeaders</td>
    <td class="tg-tcrt">16</td>
    <td class="tg-i7zr">Export line header string</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$ExportToTextFileAllHeaders</td>
    <td class="tg-tcrt">24</td>
    <td class="tg-i7zr">Export all header strings</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$ExportToTextFileCheckBoxFalse</td>
    <td class="tg-tcrt">32</td>
    <td class="tg-i7zr">Checkbox type cells that are not checked output 0</td>
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
    <td>An error occurred in the ExportToTextFileU method

</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.SaveDialog("Save", "Text File(*.txt)=*.txt", "txt", "");
    ExportToTextFileU(f, "", ",", "", $ExportToTextFileAllHeaders);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportrangetotextfileu">ExportRangeToTextFileU</a>, <a href="/package/extension5/sspread/methods/exporttotextfile">ExportToTextFile</a>, <a href="/package/extension5/sspread/methods/loadtextfile">LoadTextFile</a> method</td>
  </tr>
</table>
