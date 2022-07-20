---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Find Method
nav_order: 6
permalink: /package/csvpackage/csvdocument/methods/find
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Search CSVData under specified conditions and returns the first row index found from the rows.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = csvdoc.Find( <b>row [, cond1 [, cond2, … ] ] </b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Return row that starts from number 0 that first matches the specified condition.<br>If matches row is not found, -1 is returned.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b><i>row</i></b></td>
    <td>Return row with index 0 from row to start the search.<br>Row after specified <b><i>row</i></b> will be searched.</td>
  </tr>
  <tr>
    <td>String <b><i>cond</i></b></td>
    <td>Search condition.<br> Specify as the same format as <a href="/package/csvpackage/csvdocument/methods/load">Load</a> method.<br> Can specify as many search conditions, as long as the maximum condition is same with number of columns, and to specify more than one condition, combine them with AND.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    csvdoc << Form1.Spread1.row;
    var row = csvdoc.Find(0, "0==X11", "3n&lt;100");
    Form1.Spread1.Value = row;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/load">Load</a>, <a href="/package/csvpackage/csvdocument/methods/replace">Replace</a> methods</td>
  </tr>
</table>



