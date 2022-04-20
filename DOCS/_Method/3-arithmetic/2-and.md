---
layout: default

parent: Arithmetic Functions

title: and
nav_order: 2
permalink: /method/arithmetic/and
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Calculate the logical product of two numbers.<br>*<small>Added since Version 5.0.1</small>*<br>*<small>Cannot be used with Mobile & AI version</small>*</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var a = and (<b>arg1</b>, <b>arg2</b>)</td>
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
a = and(0x0000FFFF, 0x4000C000);    /* aは0x0000C000となる */</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/arithmetic/or">or</a>, <a href="/method/arithmetic/xor">xor</a> method</td>
  </tr>
</table>





