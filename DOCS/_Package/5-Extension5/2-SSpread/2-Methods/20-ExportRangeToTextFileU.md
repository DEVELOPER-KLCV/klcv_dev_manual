---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportRangeToTextFileU Method
nav_order: 20
permalink: /package/extension5/sspread/methods/exportrangetotextfileu
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Exports a specific range of cells to a Unicode text file using your own specified delimiter.<br><br>It has the same function as the <a href="/package/extension5/sspread/methods/exportrangetotextfile">ExportRangeToTextFile</a> method, but the output result is a Unicode text file.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportRangeToTextFileU(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>, <b>Writer</b>, <b>celldelim</b>, <b>coldelim</b>, <b>rowdelim</b>, <b>flags</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="9">Arguments</td>
    <td><b>col</b></td>
    <td>Start column number of cell range to export</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Start row number of cell range to export</td>
  </tr>
  <tr>
    <td><b>col2</b></td>
    <td>Last column number of cell range to export</td>
  </tr>
  <tr>
    <td><b>row2</b></td>
    <td>Last row number of cell range to export</td>
  </tr>
  <tr>
    <td><b>Writer</b></td>
    <td>Export destination  <a href="/base/readerwriter#writer-object">Writer Object</a></td>
  </tr>
  <tr>
    <td><b>celldelim</b></td>
    <td>Cell delimeter character</td>
  </tr>
  <tr>
    <td><b>coldelim</b></td>
    <td>Column delimiter character</td>
  </tr>
  <tr>
    <td><b>rowdelim</b></td>
    <td>Row delimiter character</td>
  </tr>
  <tr>
    <td><b>flags</b></td>
    <td>Method to create a file<br>Specify a combination of the following values.<br><style type="text/css">
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
    <td class="tg-0pky">$ExportRangeToTextFileUnformattedData</td>
    <td class="tg-c3ow">4</td>
    <td class="tg-0pky">Export as unformatted data</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ExportRangeToTextFileColHeaders</td>
    <td class="tg-c3ow">8</td>
    <td class="tg-0pky">Export column header string</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ExportRangeToTextFileRowHeaders</td>
    <td class="tg-c3ow">16</td>
    <td class="tg-0pky">Export line header string</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ExportRangeToTextFileAllHeaders</td>
    <td class="tg-c3ow">24</td>
    <td class="tg-0pky">Export all header strings</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ExportRangeToTextFileCheckBoxFalse</td>
    <td class="tg-c3ow">32</td>
    <td class="tg-0pky">Checkbox type cells that are not checked output 0</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-25</td>
    <td>	No valid Writer object specified</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>	An error occurred in the ExportRangeToTextFileU method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.SaveDialog("Save", "Text File(*.txt)=*.txt", "txt", "");
    ExportRangeToTextFileU(1, 1, 10, 10, f, "", ",", "", $ExportToTextFileAllHeaders);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportrangetotextfile">ExportRangeToTextFile</a>, <a href="/package/extension5/sspread/methods/exportrangetotextfileu">ExportToTextFileU</a>, <a href="/package/extension5/sspread/methods/loadtextfile">LoadTextFile</a> methods</td>
  </tr>
</table>
