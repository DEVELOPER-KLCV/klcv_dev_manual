---
layout: default

grand_parent: FlexView Class
parent: Methods
has_children: false
title: FlexView.DeleteRow Method
nav_order: 2
permalink: /package/extension4/flexview/flexview/methods/deleterows
---
# {{ page.title }}

<table> 
  <tr>
    <td>Explanation</td>
    <td colspan="2">Delete the row at the specified position</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var row = FlexView1.DeleteRow( <b><i>position</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a reference to the <a href="/package/extension4/flexview/flexrow">FlexRow</a> object that points to the next row after the deleted row.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>position</i></b></td>
    <td>Specify the position to delete with a line number starting from 0.</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-6</td>
    <td>FlexRecord not found</td>
  </tr>
    <tr>
    <td>EXT-13</td>
    <td>Row not found</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
      var row = FlexView1.GetRow();
      while (!row.End) {
          if (row.item1.Value == "X") {
              row = FlexView1.DeleteRow(row.Position);
          } else {
              row.MoveNext();
          }
      }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>