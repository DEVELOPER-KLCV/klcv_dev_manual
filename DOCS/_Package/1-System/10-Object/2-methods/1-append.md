---
layout: default

grand_parent: Object Class
parent: Methods
has_children: false
title: Object.Append Method
nav_order: 1
permalink: /package/system/object/methods/append
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.Append( child [, name ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Object <b>child</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>name</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="5">Exception</td>
    <td>CRS-334</td>
    <td></td>
  </tr>
  <tr>
    <td>CRS-335</td>
    <td></td>
  </tr>
  <tr>
    <td>CRS-336</td>
    <td></td>
  </tr>
  <tr>
    <td>CRS-357</td>
    <td></td>
  </tr>
  <tr>
    <td>CRS-362</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>Function OnTouch(e) {
    var child = new Array(1, 2, 3, 4, 5);
    Append(child, "TheArray");
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/object/methods/delete">Delete</a>, <a href="/package/system/object/methods/deletechild">DeleteChild</a> methods</td>
  </tr>
</table>



