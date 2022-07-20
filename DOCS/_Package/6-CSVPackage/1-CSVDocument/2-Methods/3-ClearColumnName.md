---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.ClearColumnName Method
nav_order: 3
permalink: /package/csvpackage/csvdocument/methods/clearcolumnname
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Delete all column names.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.ClearColumnName( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
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
    csvdoc.ClearColumnName();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/getcolumnname">GetColumnName</a>, <a href="/package/csvpackage/csvdocument/methods/setcolumnname">SetColumnName</a> methods</td>
  </tr>
</table>



