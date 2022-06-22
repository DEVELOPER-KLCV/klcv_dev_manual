---
layout: default

grand_parent: FlexRow Class
parent: Methods
has_children: false
title: FlexRow.GetHeaderColumn Method
nav_order: 2
permalink: /package/extension4/flexview/flexrow/methods/getheadercolumn
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns a reference to the FlexCell object at the specified location. <br>Unlike GetColumn, the position is specified with the leftmost header column as 0, and both the header column and the data column can be obtained. <br>If the InvalidState property is $ TRUE, the exception EXT-12 is raised.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var col = row.GetHeaderColumn( <b><i>pos</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">If the FlexCell can be obtained successfully, the FlexCell reference is returned. If it cannot be obtained, it returns null.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>pos</i></b></td>
    <td>Specify a column number starting from 0. For the column number, specify 0 for the first header column and 1 for the next header column. The data column is specified by the serial number in the header.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-12</td>
    <td>Invalid accessor</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var row = FlexView1.GetRow();
    var key = null;
    var sum = 0;
    while (!row.End) {
        var col = row.GetHeaderColumn(1);
        col.BgColor = $STD;
        row.MoveNext();
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>