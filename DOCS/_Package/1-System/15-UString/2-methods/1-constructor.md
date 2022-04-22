---
layout: default

grand_parent: UString Class
parent: Properties
has_children: false
title: UString Constructor
nav_order: 1
permalink: /package/system/ustring/methods/constructor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Initialize the UString object.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var str = new UString( [ <b>text_1</b> [, <b>text_2</b> [, … ] ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">UString object</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>UString <b>text_n</b></td>
    <td>Value to initialize<br>If you specify more than one, it will be initialized with the concatenated character string.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new UString("ABC", "DEF");
print(str, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>