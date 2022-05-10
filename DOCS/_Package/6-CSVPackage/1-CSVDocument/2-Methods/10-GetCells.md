---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.GetCells Method
nav_order: 10
permalink: /package/csvpackage/csvdocument/methods/getcells
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.GetCells( <b>row [, startcol [, endcol ] ] </b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>startcol</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>endcol</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CSV-13</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    csvdoc.Load(robj);
    
    /* Get the 3rd to 5th columns of the 2nd row */
    var cells = csvdoc.GetCells(1, 2, 5);
    for (var i = 0; i < cells.Length; i++) {
        print(cells[i], "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/setcells">SetCells</a>, <a href="/package/csvpackage/csvdocument/methods/getcell">GetCell</a> methods</td>
  </tr>
</table>



