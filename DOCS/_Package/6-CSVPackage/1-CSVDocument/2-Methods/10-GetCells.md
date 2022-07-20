---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument.GetCells Method
nav_order: 10
permalink: /package/csvpackage/csvdocument/methods/getcells
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Collects data in multiple columns of the specified row at once.<br><small><span style="color:red">Added since Ver.4.1.2, Mobile Ver.3.0.0 </span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">csvdoc.GetCells( <b>row [, startcol [, endcol ] ] </b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Array of String objects of the retrieved cells</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b><i>row</i></b></td>
    <td>Retrieved row that starts form 0 row index</td>
  </tr>
  <tr>
    <td>integer <b><i>startcol</i></b></td>
    <td>Start retrieval with column that start with index column 0<br>If the <b><i>startcol</i></b> is greater than the number of columns that actually exist, no columns will be retrieved. If <b><i>startcol</i></b> is omitted or a negative number is specified, the first column will be retrieved.</td>
  </tr>
  <tr>
    <td>integer <b><i>endcol</i></b></td>
    <td>End retrieval with column that start with index column 0<br>The columns before the specified column are retrieved up to one column.If <b><i>endcol</i></b> is less than <b><i>startcol</i></b>, no column is retrieved.If <b><i>endcol</i></b> is omitted or a value greater than the number of columns actually present is specified, the last column is retrieved.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CSV-13</td>
    <td>Incorrect row index</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument;
    csvdoc.Load(robj);
    
    /* Get the 3rd to 5th columns of the 2nd row */
    var cells = csvdoc.GetCells(1, 2, 5);
    for (var i = 0; i < cells.Length; i++) {
        print(cells[i], "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/csvpackage/csvdocument/methods/setcells">SetCells</a>, <a href="/package/csvpackage/csvdocument/methods/getcell">GetCell</a> methods</td>
  </tr>
</table>



