---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportRangeToXML Method
nav_order: 21
permalink: /package/extension5/sspread/methods/exportrangetoxml
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Export a specific range of cells to an XML file.<br><br>A cell range specification has been added to the functionality of the <a href="/package/extension5/sspread/methods/exporttoxml">ExportToXML</a> method.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportRangeToXML(<b>col</b>, <b>row</b>, <b>col2</b>, <b>row2</b>, <b>Writer</b>, <b>root</b>, <b>collection</b>, <b>flags</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="8">Arguments</td>
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
    <td>Export destination Writer object</td>
  </tr>
  <tr>
    <td><b>root</b></td>
    <td>Root element name used for XML file</td>
  </tr>
  <tr>
    <td><b>collection</b></td>
    <td>Collection element name used for XML file</td>
  </tr>
  <tr>
    <td><b>flags</b></td>
    <td>Specify whether to export formatted data<br>Specify the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">Constant</th>
    <th class="tg-c3ow">Value</th>
    <th class="tg-0pky">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$ExportToXMLFormattedData</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">Export as formatted data</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ExportToXMLUnFormattedData</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">Export as unformatted data</td>
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
    <td>An error occurred in the ExportRangeToXML method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.SaveDialog("Save", "XML File(*.xml)=*.xml", "xml", "");
    ExportRangeToXML(1, 1, 10, 10, f, "root", "collection", $ExportToXMLFormattedData);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exporttoxml">ExportToXML</a> method</td>
  </tr>
</table>
