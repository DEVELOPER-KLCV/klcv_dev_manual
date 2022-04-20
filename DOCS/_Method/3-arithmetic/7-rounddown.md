---
layout: default

parent: Arithmetic Functions

title: rounddown
nav_order: 7
permalink: /method/arithmetic/rounddown
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Truncate at the specified digit.<br><br>If the number of digits is positive, the digits after the decimal point are truncated.<br>If the number of digits is negative, the integer part is truncated at the specified digit.<br>When the digit is omitted, the number after the decimal point is truncated.<br><br>Rounddown of the rounddown function (when the number of digits = 0) will be <b>Maximum (positive direction) of integers less than or equal to the value</b><br>*<small>Added since Version 2.0.0</small>*</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var r = rounddown( <b>arg</b>, <b>n</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a number rounded down to the specified digit.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Number <b>arg</b></td>
    <td>Original number</td>
  </tr>
  <tr>
    <td>Number <b>n</b></td>
    <td> Position of the digit to be truncated</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>print(rounddown(12345.678, -2)); /* 12300となる */
print(rounddown(12345.678));     /* 12345となる */
print(rounddown(12345.678, 2));  /* 12345.67となる */
 
print(rounddown(0.50));  /* 0となる */
print(rounddown(-0.50)); /* -1となる */</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/arithmetic/round">round</a>, <a href="/method/arithmetic/roundup">roundup</a>, <a href="/method/arithmetic/roundm">roundm</a> methods</td>
  </tr>
</table>





