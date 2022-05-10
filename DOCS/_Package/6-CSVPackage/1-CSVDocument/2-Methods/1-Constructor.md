---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument Constructor
nav_order: 1
permalink: /package/csvpackage/csvdocument/methods/constructor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var csvdoc = new CSVDocument( [ <b>enc</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">CSVDocument object</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>enc</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument(CSVDocument.Unicode);
    var res = session.Get("/test/sample.csv");
    csvdoc.Load(res);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



