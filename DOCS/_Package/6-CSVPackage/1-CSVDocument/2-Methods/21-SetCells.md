---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.SetCells Method
nav_order: 21
permalink: /package/csvpackage/csvdocument/methods/setcells
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.SetCells( <b>row, column [, data1 [, data2 ... ] ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>data</b></td>
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
    csvdoc.Load(robj);
    
    /* Set "a" in the 3rd column of the 2nd row, "b" in the 4th column, and "c" in the 5th column. */
    csvdoc.SetCells(1, 2, "a", "b", "c");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/getcells">GetCells</a>, <a href="/package/csvpackage/csvdocument/methods/setcell">SetCell</a> methods</td>
  </tr>
</table>



