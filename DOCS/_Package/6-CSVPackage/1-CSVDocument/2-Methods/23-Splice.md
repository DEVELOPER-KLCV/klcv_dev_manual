---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Splice Method
nav_order: 23
permalink: /package/csvpackage/csvdocument/methods/splice
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Split CSV data according to the specified conditions.<br><br>Rows that setisfy the condition are removed from the CSVDocument object and stored in a new CSVDocument object.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var csvdoc2 = csvdoc.Splice( <b>row [, cond1 [, cond2, … ] ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">A new CSVDocument object consisting of only rows that satisfy the condition.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>row</b></td>
    <td>Line number starting with 0 of the line that starts the split.<br><br>The <b>row</b> after the row specified by row is the target of division.</td>
  </tr>
  <tr>
    <td>String  <b>cond</b></td>
    <td>Search conditions that specify the lines to be split<br><br>Specify in the same format as the Load method.<br><br>Can be specified as many search conditions as the number of columns at the maximum, and if multiple search conditions specified, combine them with AND.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    /* Rows where the first column is numeric and greater than 2001 and the second column is blank are stored in csvdoc2. */
    /* The other lines remain in csvdoc1. */
    var csvdoc1 = new CSVDocument;
    csvdoc1.Get("http://server/data1.csv");
    var csvdoc2 = csvdoc1.Splice(0, "0n>2001", "1==");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/merge">Merge</a>, <a href="/package/csvpackage/csvdocument/methods/load">Load</a> methods</td>
  </tr>
</table>



