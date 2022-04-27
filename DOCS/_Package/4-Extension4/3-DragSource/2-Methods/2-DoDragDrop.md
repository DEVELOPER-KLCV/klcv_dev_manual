---
layout: default

grand_parent: DragSource Class
parent: Methods
has_children: false
title: DragSource.DoDragDrop Method
nav_order: 2
permalink: /package/extension4/dragsource/methods/dodragdrop
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">source.DoDragDrop( [ <b>type</b> [, <b>waitTime</b> [, <b>margin</b> ] ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b>type</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>waitTime</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>margin</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    source.SetString("Drag and Drop");
    source.DoDragDrop($MOVEMODE, 10, 8);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>