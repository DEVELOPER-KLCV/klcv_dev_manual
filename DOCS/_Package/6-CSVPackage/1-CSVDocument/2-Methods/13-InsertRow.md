---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.InsertRow Method
nav_order: 13
permalink: /package/csvpackage/csvdocument/methods/insertrow
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Inserts a row at the specified position.<br>The data in each cell of the inserted row is initialised with an empty string.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.InsertRow( <b>row </b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>row</b></td>
    <td>Line number starting with 0 at the insertion position.<br>Specify 0 to create the first line, 1 to create a new line at the second line. Specifying -1 or a number greater than the current line number inserts it as the last line.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    csvdoc.InsertColumn(-1);
    csvdoc.InsertColumn(-1);
    csvdoc.InsertRow(-1);
    csvdoc.InsertRow(-1);
    csvdoc.SetCell(1, 1, "sample");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/deleterow">DeleteRow</a>, <a href="/package/csvpackage/csvdocument/methods/insertcolumn">InsertColumn</a>, <a href="/package/csvpackage/csvdocument/methods/deletecolumn">DeleteColumn</a> methods</td>
  </tr>
</table>



