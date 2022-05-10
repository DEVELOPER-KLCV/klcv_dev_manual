---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Save Method
nav_order: 18
permalink: /package/csvpackage/csvdocument/methods/save
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.Save( <b>writer [, cond1 [, cond2, … ] ]</b> )<br><br>**<small>Since Version 5.0.3, the following formats are possible</small>**<br>csvdoc.Save( <b>writer [, delimiter [, cond1 [, cond2, … ] ] ] </b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>Object <b>writer</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>delimiter</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>cond</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>CSV-11</td>
    <td></td>
  </tr>
  <tr>
    <td>CSV-12</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    var res = session.Get("http://server/sample.csv");
    csvdoc.Load(res);
    var fs = new FileSystem;
    var fp = fs.Open("sample.csv", FileSystem.OPEN_WRITE);
    csvdoc.Save(fp);
    fp.Close();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/load">Load</a> method</td>
  </tr>
</table>



