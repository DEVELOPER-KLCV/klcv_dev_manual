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
    <td colspan="2">Set the name of the column.<br><br>Column names can represent object names and property names, as well as simply used as names, and can be copied when copying CSV data to an array with the <a href="/package/csvpackage/csvdocument/operators/1">[] << CSV constant operator</a> or  <a href="/package/csvpackage/csvdocument/operators/2">[] << CSVDocument operator</a>. The destination object or property can be explicitly specified.
    <br></td>
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
    <td>Column number 0 to set the name of column</td>
  </tr>
  <tr>
    <td>String  <b>name</b></td>
    <td>Column name<br><br>If empty string is specified, the column name will be deleted.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CSV-14</td>
    <td>Incorrect column index</td>
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



