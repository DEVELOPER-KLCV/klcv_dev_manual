---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Merge Method
nav_order: 15
permalink: /package/csvpackage/csvdocument/methods/merge
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Merge two CSV data.<br>The number of columns in the two merged CSV data will be adjusted to the larger one.<br><br><small><span style="color:red">Added since Ver.4.1.0. Same functionality as in previous versions of <i>marge</i>.</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var csvdoc3 = csvdoc2.Merge( <b>csvdoc</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">New CSVDocument object combined from two CSVDocument</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>CSVDocument <b>csvdoc</b></td>
    <td>CSVDocument object to be combined</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>CSV-15</td>
    <td>The argument is not valid CSVDocument object</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc1 = new CSVDocument;
    var csvdoc2 = new CSVDocument;
    csvdoc1.Get("http://server/data1.csv");
    csvdoc2.Get("http://server/data2.csv");
    var csvdoc3 = csvdoc1.Merge(csvdoc2);
    csvdoc3.Save(file);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/splice">Splice</a> method</td>
  </tr>
</table>



