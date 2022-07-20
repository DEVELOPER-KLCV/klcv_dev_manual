---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.Truncate Method
nav_order: 25
permalink: /package/csvpackage/csvdocument/methods/truncate
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Delete multiple rows at once. The column is maintained.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.Truncate( [ <b>row</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>row</b></td>
    <td>Line number starting with 0 on the line that starts the deletion.<br>The rows after the specified <b>row</b> will be  deleted. If omitted, all lines will be deleted.<br><small><span style="color:red">Added since Ver.4.1.3, Mobile Ver.3.0.0</span></small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CSV-13</td>
    <td>Incorrect row index.</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    var res = session.Get("/test/sample.csv");
    csvdoc.Load(res);
    csvdoc.Truncate(5);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/clear">Clear</a> method</td>
  </tr>
</table>



