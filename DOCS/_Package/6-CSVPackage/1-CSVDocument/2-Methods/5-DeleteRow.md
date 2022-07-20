---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.DeleteRow Method
nav_order: 5
permalink: /package/csvpackage/csvdocument/methods/DeleteRow
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Delete row of selected row index.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.DeleteRow( <b><i>row </i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>row</i></b></td>
    <td>Line number starting with 0 on the line to be deleted.<br>If you specify 0, the first line is deleted, and if you specify 1, the second line is deleted.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CSV-6</td>
    <td>Specified row cannot be deleted</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    var res = session.Get("/test/sample.csv");
    csvdoc.Load(res);
    csvdoc.DeleteRow(0);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/insertrow">InsertRow</a>, <a href="/package/csvpackage/csvdocument/methods/insertcolumn">InsertColumn</a>, <a href="/package/csvpackage/csvdocument/methods/deletecolumn">DeleteColumn</a> methods</td>
  </tr>
</table>



