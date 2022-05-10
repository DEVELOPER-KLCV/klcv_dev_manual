---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Load Method
nav_order: 14
permalink: /package/csvpackage/csvdocument/methods/load
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.Load( <b>reader [, cond1 [, cond2, … ] ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Object <b>reader</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>cond</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>CSV-8</td>
    <td></td>
  </tr>
  <tr>
    <td>CSV-9</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    var res = session.get("/test/sample.csv");
    csvdoc.Load(res, "1n>100", "2==[3]");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/save">Save</a>, <a href="/package/csvpackage/csvdocument/methods/get">Get</a>, <a href="/package/csvpackage/csvdocument/methods/parse">Parse</a> methods</td>
  </tr>
</table>



