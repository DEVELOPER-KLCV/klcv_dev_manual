---
layout: default

grand_parent: FlexView Class
parent: Methods
has_children: false
title: FlexView.InsertRow Method
nav_order: 6
permalink: /package/extension4/flexview/flexview/methods/insertrow
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Add a row at the specified position</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var row = FlexView1.InsertRow( [ <b><i>count</i></b> [, <b><i>position</i></b> ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a reference to the <a href="/package/extension4/flexview/flexrow">FlexRow</a> object that points to the first row inserted.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b><i>count</i></b></td>
    <td>Specify the number of lines to insert. If omitted, one line will be added.</td>
  </tr>
    <tr>
    <td>integer <b><i>position</i></b></td>
    <td>Specify the insertion position with a line number starting from 0. -1 or if omitted, it will be added at the end.</td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>EXT-1</td>
    <td>Invalid argument</td>
  </tr>
    <tr>
    <td>EXT-6</td>
    <td>FlexRecord not found</td>
  </tr>
      <tr>
    <td>EXT-13</td>
    <td>Column not found</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var row = FlexView1.InsertRow(10);
    for (var i = 0; i < 10; i++) {
        row.item1.Value = "a";
        row.MoveNext();
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>