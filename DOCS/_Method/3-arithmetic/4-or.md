---
layout: default

parent: Arithmetic Functions

title: or
nav_order: 4
permalink: /method/arithmetic/or
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Find the logical sum of the two numbers.<br>*<small>Added since Version 5.0.1</small>*<br>*<small>Cannot be used with Mobile & AI version</small>*</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = or( <b>arg1</b>, <b>arg2</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Calculation result</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Number <b>arg1</b></td>
    <td>The target number. It is automatically converted to a 32-bit integer internally.</td>
  </tr>
  <tr>
    <td>Number <b>arg2</b></td>
    <td>The target number. It is automatically converted to a 32-bit integer internally.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var a;
a = or(0x40000000, 0x0000C000);    /* aは0x4000C000となる */</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/arithmetic/and">and</a>, <a href="/method/arithmetic/xor">xor</a> method</td>
  </tr>
</table>





