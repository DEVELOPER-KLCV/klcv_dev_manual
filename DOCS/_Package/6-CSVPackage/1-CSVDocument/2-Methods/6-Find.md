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
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = csvdoc.Find( <b>row [, cond1 [, cond2, … ] ] </b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>cond</b></td>
    <td></td>
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



