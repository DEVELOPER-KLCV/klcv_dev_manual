---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.GetCellByName Method
nav_order: 9
permalink: /package/csvpackage/csvdocument/methods/getcellbyname
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var data = csvdoc.GetCellByName( <b>row, columnName </b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>columnName </b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>CSV-13</td>
    <td></td>
  </tr>
  <tr>
    <td>CSV-14</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    csvdoc.Get("/test/sample.csv");
    csvdoc.SetColumnName(2, "Type");
    var cell = csvdoc.GetCellByName(0, "Type");
    print(cell, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/setcellbyname">SetCellByName</a>, <a href="/package/csvpackage/csvdocument/methods/getcell">GetCell</a>, <a href="/package/csvpackage/csvdocument/methods/getcolumnname">GetColumnName</a>, <a href="/package/csvpackage/csvdocument/methods/setcolumnname">SetColumnName</a> methods</td>
  </tr>
</table>



