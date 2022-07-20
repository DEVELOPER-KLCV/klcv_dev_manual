---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.DeleteColumn Method
nav_order: 4
permalink: /package/csvpackage/csvdocument/methods/DeleteColumn
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Delete column of selected column index</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.DeleteColumn( <b><i>column</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>column</i></b></td>
    <td>Delete column that starts from index column 0<br>If specified 0,the first column will be deleted,<br>if specified 1, the second column will be deleted.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CSV-4</td>
    <td>Specified column cannot be deleted</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    var res = session.get("/test/sample.csv");
    csvdoc.Load(res);
    csvdoc.DeleteColumn(0);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/insertcolumn">InsertColumn</a>, <a href="/package/csvpackage/csvdocument/methods/insertrow">InsertRow</a>, <a href="/package/csvpackage/csvdocument/methods/deleterow">DeleteRow</a> methods</td>
  </tr>
</table>



