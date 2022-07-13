---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportToXML Method
nav_order: 28
permalink: /package/extension5/sspread/methods/exporttoxml
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Export the spreadsheet to an XML file. <br><br>The column header is used as a child element within each collection element in XML. All row headers are ignored.<br><br> Use the <a href="/package/extension5/sspread/methods/exportrangetoxml">ExportRangeToXML</a> method to export a specific cell range.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ExportToXML(<b>Writer</b>, <b>root</b>, <b>collection</b>, <b>flags</b>)</td>
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
    <td><b>root</b></td>
    <td>	
Root element name used for XML file</td>
  </tr>
  <tr>
    <td><b>collection</b></td>
    <td>Collection element name used for XML file</td>
  </tr>
  <tr>
    <td><b>flags</b></td>
    <td>Specify whether to export formatted data<br> Specify the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
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
    <td class="tg-j5n6">$ExportToXMLFormattedData</td>
    <td class="tg-lcf4">0</td>
    <td class="tg-j5n6">Export as formatted data</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$ExportToXMLUnFormattedData</td>
    <td class="tg-lcf4">1</td>
    <td class="tg-j5n6">Export as unformatted data</td>
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
    <td>An error occurred in the ExportToXML method

</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem();
    var f = fs.SaveDialog("Save", "XML File(*.xml)=*.xml", "xml", "");
    ExportToXML(f, "root", "collection", $ExportToXMLFormattedData);
    f.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/exportrangetoxml">ExportRangeToXML</a> method</td>
  </tr>
</table>
