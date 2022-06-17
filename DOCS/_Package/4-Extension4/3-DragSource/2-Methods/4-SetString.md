---
layout: default

grand_parent: DragSource Class
parent: Methods
has_children: false
title: DragSource.SetString Method
nav_order: 4
permalink: /package/extension4/dragsource/methods/setstring
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the character string data to be dragged and dropped. If it is already set, it will be overwritten.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">source.SetString( <b><i>str</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b><i>str</i></b></td>
    <td>Character string data to be dragged and dropped. If it is an empty string, it will be ignored.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>CRS-112</td>
    <td>Cannot be converted to a string</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    source.SetString("Drag and Drop");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>