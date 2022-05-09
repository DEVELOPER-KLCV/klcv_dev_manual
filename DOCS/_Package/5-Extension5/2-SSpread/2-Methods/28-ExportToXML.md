---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ExportToXML Method
nav_order: 28
permalink: /package/extension5/sspread/methods/ExportToXML
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
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
    <td></td>
  </tr>
  <tr>
    <td><b>root</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>collection</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>flags</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-25</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td></td>
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
