---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.DeleteCols Method
nav_order: 13
permalink: /package/extension5/sspread/methods/deletecols
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Deletes the specified column or column range.<br><br>Deleting a column does not reduce the number of columns set in the <a href="/package/extension5/sspread/properties/maxcols">MaxCols</a> property, it automatically adds a blank column at the end of the spreadsheet.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">DeleteCols(<b>col</b>, <b>numcols</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td>First column number in the range of columns to delete</td>
  </tr>
  <tr>
    <td><b>numcols</b></td>
    <td>Number of columns to delete</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>Invalid DeleteCols argument</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the DeleteCols method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Function OnRClicked(e) {
        if (e.Row == 0 && e.Col > 0) {
            var ret = PopupMenu("Insert column", "Delete column");
            switch (ret) {
            case 1:
                InsertCols(e.Col, 1);
                break;
            case 2:
                DeleteCols(e.Col, 1);
                break;
            }
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/maxcols">MaxCols</a> property<br><a href="/package/extension5/sspread/methods/deleterows">DeleteRows</a>, <a href="/package/extension5/sspread/methods/insertcols">InsertCols</a> methods</td>
  </tr>
</table>
