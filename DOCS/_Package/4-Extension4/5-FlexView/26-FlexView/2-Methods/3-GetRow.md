---
layout: default

grand_parent: FlexView Class
parent: Methods
has_children: false
title: FlexView.GetRow Method
nav_order: 3
permalink: /package/extension4/flexview/flexview/methods/getrow
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the object to drag and drop.<br> If it is already set, it will be overwritten.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">source.SetObject( <b><i>obj</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Object <b><i>obj</i></b></td>
    <td>Objects to drag and drop</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>CRS-328</td>
    <td>Only objects or properties can be converted</td>
  </tr>
    <tr>
    <td>CRS-130</td>
    <td>Unable to convert</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var rec = new Record {
       String s;
       Number n;
    }
    source.SetObject(rec);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>
