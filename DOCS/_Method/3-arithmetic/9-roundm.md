---
layout: default

parent: 3. Arithmetic Functions

title: roundm
nav_order: 9
permalink: /method/arithmetic/roundm
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Rounds the original value to be a multiple of the specified value.<br>If you specify a value greater than 0 for the rounding method, it will be rounded up.<br>If 0 is specified or omitted for the rounding method, rounding is performed.<br>If you specify a negative number for the rounding method, it will be rounded down.<br>*<small>Added since Mobile Version 2.0.0</small>*</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var r = roundm( <b>arg</b>, <b>n</b>, <b>m</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a number rounded to a multiple of the specified value.</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>Number <b>arg</b></td>
    <td>Original number</td>
  </tr>
  <tr>
    <td>Number <b>n</b></td>
    <td> Numerical value for rounding</td>
  </tr>
  <tr>
    <td>Number <b>m</b></td>
    <td>Rounding method</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var b;
b = 50.67;
a = roundm(b, 10, 1);  /* aは60となる */
a = roundm(b, 10);     /* aは50となる */
a = roundm(b, 10, -1); /* aは50となる */</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/arithmetic/round">round</a>, <a href="/method/arithmetic/rounddown">rounddown</a>, <a href="/method/arithmetic/roundup">roundup</a> methods</td>
  </tr>
</table>





