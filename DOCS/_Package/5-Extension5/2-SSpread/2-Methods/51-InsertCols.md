---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.InsertCols Method
nav_order: 51
permalink: /package/extension5/sspread/methods/insertcols
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Inserts one or more columns before the specified column.<br><br>Inserting columns does not increase the maximum number of columns set in the <a href="/package/extension5/sspread/properties/maxcols">MaxCols</a> property.<br>The data that was set in the last column of the spreadsheet will be out of range and lost due to the insertion of the column.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">InsertCols(<b>col</b>, <b>numcols</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td>Column number immediately before the column insertion position</td>
  </tr>
  <tr>
    <td><b>numcols</b></td>
    <td>Number of columns to insert</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>The argument of InsertCols is invalid</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the InsertCols method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Function OnRClicked(e) {
        if (e.Row == 0 && e.Col > 0) {
            var ret = PopupMenu("Add row", "Delete row");
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/maxcols">MaxCols</a> property<br><a href="/package/extension5/sspread/methods/deletecols">DeleteCols</a>, <a href="/package/extension5/sspread/methods/insertrows">InsertRows</a> methods</td>
  </tr>
</table>
