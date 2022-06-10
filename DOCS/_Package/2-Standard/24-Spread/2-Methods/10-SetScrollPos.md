---
layout: default

grand_parent: Spread Class
parent: Methods
has_children: false
title: Spread.SetScrollPos Method
nav_order: 10
permalink: /package/standard/spread/methods/setscrollpos
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the scroll position.<br>Scrolls to the position where the <b><i>row</i></b> specified by row appears in the display area (not the first row, but as much as necessary for display).<br><br>Since ver3.1.2.0, <b><i>col</i></b> can be specified. Scrolls so that the cells specified by <b><i>row</i></b> and <b><i>col</i></b> are included in the display range.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">Spread1.SetScrollPos( <b><i>row</i></b> [, <b><i>col</i></b>> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b><i>row</i></b></td>
    <td>row position<br>0 is the top line. Every time the value increases by 1, it goes down one row.</td>
  </tr>
  <tr>
    <td>integer <b><i>col</i></b></td>
    <td>column position<br>0 is the leftmost column. Every time the value increases by 1, it becomes one column to the right.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/spread/methods/GetScrollPos">GetScrollPos</a> method</td>
  </tr>
</table>



