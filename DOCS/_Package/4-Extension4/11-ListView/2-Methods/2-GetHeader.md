---
layout: default

grand_parent: ListView Class
parent: Methods
has_children: false
title: ListView.GetHeader Method
nav_order: 2
permalink: /package/extension4/listview/methods/getheader
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns a reference to the column header information.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ref = ListView1.GetHeader( <b><i>num</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">ListViewHeader Reference</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>num</i></b></td>
    <td>Column number (0-xx)</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var hlv = ListView1.GetHeader(0);
    hlv.Title = "Name";
    hlv.Width = 50;
    
    ※See the ListViewHeader section for settings.
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>