---
layout: default

grand_parent: DragSource Class
parent: Methods
has_children: false
title: DragSource.AddFile Method
nav_order: 1
permalink: /package/extension4/dragsource/methods/addfile
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the file to drag and drop. The file to be dragged and dropped is added each time this method is executed.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">source.AddFile( <b><i>filepath</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b><i>filepath</i></b></td>
    <td>Absolute path of the file to drag and drop. If it is an empty string, it will be ignored.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CRS-112</td>
    <td>Cannot be converted to a string</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    source.AddFile("C:\\app\\userdata.txt");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>