---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Parse Method
nav_order: 16
permalink: /package/csvpackage/csvdocument/methods/parse
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Load CSV data from character string<br><br><small><span style="color:red">Added since Ver.4.0.0, Mobile Ver.3.0.0</span></small><br><br>When Parse method is executed, the previous data will be lost.<br><br>The loading function of Parse method is same as <a href="/package/csvpackage/csvdocument/methods/load">Load</a> method, but a String object can be specified as an argument.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.Parse( <b>str [, cond1 [, cond2, … ] ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>str</b></td>
    <td>CSV character string</td>
  </tr>
  <tr>
    <td>String <b>cond</b></td>
    <td>Search condition that specify the rows to be loaded.<br>To set this, write the format same as <a href="/package/csvpackage/csvdocument/methods/load">Load</a>method.<br>For the Search condition, the Maximum can be specified only as the same number with the number of columns. If more than one is specified, combine them with AND.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    var str = "aaa,bbb,ccc";
    csvdoc.Parse(str);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/save">Save</a>, <a href="/package/csvpackage/csvdocument/methods/get">Get</a>, <a href="/package/csvpackage/csvdocument/methods/load">Load</a> methods</td>
  </tr>
</table>



