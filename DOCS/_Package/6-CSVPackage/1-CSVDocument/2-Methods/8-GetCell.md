---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.GetCell Method
nav_order: 8
permalink: /package/csvpackage/csvdocument/methods/getcell
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify the row and column,then data of the corresponding cell wiil be retrieved.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var data = csvdoc.GetCell( <b><i>row, column</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Character string of cell <br>If the corresponding cell does not exist, null is returned.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b><i>row</i></b></td>
    <td>Retrieve cell which row starts from 0</td>
  </tr>
  <tr>
    <td>integer <b><i>column</i></b></td>
    <td>Retrieve cell which column starts from 0</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    var res = session.Get("/test/sample.csv");
    csvdoc.Load(res);
    var cell = csvobj.GetCell(0, 1);
    print(cell, "\n");   
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/setcell">SetCell</a>, <a href="/package/csvpackage/csvdocument/methods/getcells">GetCells</a>, <a href="/package/csvpackage/csvdocument/methods/getcellbyname">GetCellByName</a> methods</td>
  </tr>
</table>



