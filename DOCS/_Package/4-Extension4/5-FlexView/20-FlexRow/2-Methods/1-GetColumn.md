---
layout: default

grand_parent: FlexRow Class
parent: Methods
has_children: false
title: FlexRow.GetColumn Method
nav_order: 1
permalink: /package/extension4/flexview/flexrow/methods/getcolumn
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns a reference to the FlexCell object at the specified location.<br> The GetColumn method can get the data column excluding the header column. Use the GetHeaderColumn method to get the header column.<br> If the InvalidState property is $TRUE, the exception EXT-12 is raised.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var col = row.GetColumn( <b><i>pos</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">If the FlexCell can be obtained successfully, the FlexCell reference is returned. <br>If it cannot be obtained, it returns null.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>pos</i></b></td>
    <td>Specify the column number starting from 0 for the leftmost data excluding the header column.</td>
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
        var col = row.GetColumn(1);
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