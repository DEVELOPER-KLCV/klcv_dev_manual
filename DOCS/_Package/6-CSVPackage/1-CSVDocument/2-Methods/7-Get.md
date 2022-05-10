---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Get Method
nav_order: 7
permalink: /package/csvpackage/csvdocument/methods/get
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.Get( <b>URL [, param1 [, param2, … ] ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String  <b>URL</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Object <b>param</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>CSV-1</td>
    <td></td>
  </tr>
  <tr>
    <td>CSV-10</td>
    <td></td>
  </tr>
  <tr>
    <td>CSV-331</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    csvdoc.Get("/test/sample.cgi", "KEY=126", "MODE=A");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/load">Load</a>, <a href="/package/csvpackage/csvdocument/methods/parse">Parse</a>, <a href="/package/system/netobject/methods/get">NetObject.Get</a> methods</td>
  </tr>
</table>



