---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Replace Method
nav_order: 17
permalink: /package/csvpackage/csvdocument/methods/replace
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = csvdoc.Replace( <b>row, col, val [, cond1 [, cond2, … ] ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>integer <b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>val</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>cond</b></td>
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
    csvdoc.Get("http://server/data1.csv");
    
    /* Updated the first column of every row to "new data" */
    csvdoc.Replace(0, 0, "new data");
    
    /* Update the second column of all rows to the same value as the third column */
    csvdoc.Replace(0, 1, "[2]");
    
    /* Updated the 5th column of the row where the 4th column is "1" to the same value as the 3rd column */
    csvdoc.Replace(0, 4, "[2]", "3==1");
    
    /* 6th column is the same row as 7th column, 8th column is updated to the same value as 3rd column */
    csvdoc.Replace(0, 7, "[2]", "5==[6]");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/load">Load</a>, <a href="/package/csvpackage/csvdocument/methods/find">Find</a> methods</td>
  </tr>
</table>



