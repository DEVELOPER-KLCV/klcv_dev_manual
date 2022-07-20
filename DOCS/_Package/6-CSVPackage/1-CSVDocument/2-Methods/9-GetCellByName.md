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
    <td colspan="2">To retrieve data from cell, specify the index number of row and column.<br><br>To set the column name, use <a href="/package/csvpackage/csvdocument/methods/setcolumnname">SetColumnName</a>  method or <a href="/package/csvpackage/csvdocument/csvcontants">CSVConstant</a>.<br><br><small><span style="color:red">Added since Ver.4.1.2, Mobile Ver.3.0.0</span></small> </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var data = csvdoc.GetCellByName( <b><i>row, columnName ></i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Character string of the acquired cell<br>If the corresponding cell does not exist, null is returned.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b><i>row</i></b></td>
    <td>Get row which index row start from 0</td>
  </tr>
  <tr>
    <td>String <b><i>columnName</i></b></td>
    <td>Get name of column</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>CSV-13</td>
    <td>Incorrect row index</td>
  </tr>
  <tr>
    <td>CSV-14</td>
    <td>Incorrect column index</td>
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



