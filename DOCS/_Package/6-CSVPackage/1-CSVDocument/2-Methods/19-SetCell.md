---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.SetCell Method
nav_order: 19
permalink: /package/csvpackage/csvdocument/methods/setcell
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify the row and column, and the data in the cell will be set</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.SetCell( <b>row, column, text</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b>row</b></td>
    <td>Specify cell start from row index 0</td>
  </tr>
  <tr>
    <td>integer <b>column</b></td>
    <td>Specify cell start from column index 0</td>
  </tr>
  <tr>
    <td>String <b>text</b></td>
    <td>Character string set in cell</td>
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
    csvdoc.InsertColumn(0);
    csvdoc.InsertRow(0);
    csvdoc.SetCell(0, 0, "sample");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/getcell">GetCell</a>, <a href="/package/csvpackage/csvdocument/methods/setcells">SetCells</a>, <a href="/package/csvpackage/csvdocument/methods/setcellbyname">SetCellByName</a> methods</td>
  </tr>
</table>



