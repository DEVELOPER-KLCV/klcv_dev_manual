---
layout: default

grand_parent: FlexRow Class
parent: Methods
has_children: false
title: FlexRow.MovePrev Method
nav_order: 4
permalink: /package/extension4/flexview/flexrow/methods/moveprev
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = row.MovePrev( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-12</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var row = FlexView1.GetRow();
    var key = null;
    var sum = 0;
    while (!row.End) {
        if (key != null && key != row.keyItem) {
            row.MovePrev();
            row.subTotal = sum;
            row.MoveNext();
            key = row.keyItem.ValueOf();
            sum = 0;
        }
        row.MoveNext();
    }
    row.MovePrev();
    row.subTotal = sum;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/flexview/flexrow/methods/movenext">MoveNext</a> method</td>
  </tr>
</table>