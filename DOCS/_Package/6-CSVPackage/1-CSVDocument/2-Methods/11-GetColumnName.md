---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.GetColumnName Method
nav_order: 11
permalink: /package/csvpackage/csvdocument/methods/getcolumnname
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var name = csvdoc.GetColumnName( <b>column</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>column</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CSV-14</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    csvdoc << CSV(c1,c2,c3) {
    1,2,3
    4,5,6
    };
    for (var c = 0; c < csvdoc.Columns; c++) {
        print(csvdoc.GetColumnName(c), "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/setcolumnname">SetColumnName</a>, <a href="/package/csvpackage/csvdocument/methods/clearcolumnname">ClearColumnName</a>, <a href="/package/csvpackage/csvdocument/methods/getcellbyname">GetCellByName</a>, <a href="/package/csvpackage/csvdocument/methods/setcellbyname">SetCellByName</a> methods</td>
  </tr>
</table>



