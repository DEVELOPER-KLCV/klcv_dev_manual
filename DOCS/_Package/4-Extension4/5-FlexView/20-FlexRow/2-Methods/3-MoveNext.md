---
layout: default

grand_parent: FlexRow Class
parent: Methods
has_children: false
title: FlexRow.MoveNext Method
nav_order: 3
permalink: /package/extension4/flexview/flexrow/methods/movenext
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Point to the next line. <br>It is faster than the FlexView.GetRow (n) method where you want to advance the row you want to point to. <br>If the InvalidState property is $TRUE, the exception EXT-12 is raised.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = row.MoveNext( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns true if it was successfully moved.<br> Returns false if it cannot be moved.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
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
    while (!row.End) {
        if (row.lbDeleteFlag) {
            row = FlexView1.DeleteRow(row);
        } else {
            row.MoveNext();
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/flexview/flexrow/methods/moveprev">MovePrev</a> method</td>
  </tr>
</table>