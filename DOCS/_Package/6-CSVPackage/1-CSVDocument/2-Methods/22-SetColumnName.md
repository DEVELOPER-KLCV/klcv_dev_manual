---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.SetColumnName Method
nav_order: 22
permalink: /package/csvpackage/csvdocument/methods/setcolumnname
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.SetColumnName( <b>column, name</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>column</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String  <b>name</b></td>
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
    csvdoc.Get("http://server/test.csv");
    csvdoc.SetColumnName(0, "c1");
    csvdoc.SetColumnName(1, "c2");
    csvdoc.SetColumnName(2, "c3");
    
    var csvdoc = new CSVDocument;
    csvdoc.Get("http://server/test2.csv");
    csvdoc.SetColumnName(0, ".Title");
    csvdoc.SetColumnName(1, ".Value");
    ListBox1.ListItem1 << csvdoc;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/getcolumnname">GetColumnName</a>, <a href="/package/csvpackage/csvdocument/methods/clearcolumnname">ClearColumnName</a>, <a href="/package/csvpackage/csvdocument/methods/getcellbyname">GetCellByName</a>, <a href="/package/csvpackage/csvdocument/methods/setcellbyname">SetCellByName</a> methods<br><a href="/package/csvpackage/csvdocument/operators/1">[ ] << CSV constants</a>, <a href="/package/csvpackage/csvdocument/operators/2">[ ] << CSVDocument</a> operators</td>
  </tr>
</table>



