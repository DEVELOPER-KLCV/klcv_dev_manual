---
layout: default

parent: Arithmetic Functions

title: roundup
nav_order: 8
permalink: /method/arithmetic/roundup
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Rounds up to the specified digit.<br><br>If the digit position to be rounded up is positive, it will be rounded up to the specified digit after the decimal point.<br>If the digit position to be rounded up is negative, the integer part is rounded up to the specified digit.<br>When the digit position to be rounded up is omitted, the number after the decimal point is rounded up.<br><br>Rounding up the roundup function (when the number of digits = 0) will be <b>the smallest (negative direction) of integers greater than or equal to the value</b><br>*<small>Added since Version 2.0.0</small>*</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var r = roundup( <b>arg</b>, <b>n</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a number rounded up to the specified digit.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Number <b>arg</b></td>
    <td>Original number</td>
  </tr>
  <tr>
    <td>Number <b>n</b></td>
    <td>Position of the girder to round up</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>print(roundup(12345.678, -2)); /* 12400となる */
print(roundup(12345.678));     /* 12346となる */
print(roundup(12345.678, 2));  /* 12345.68となる */
 
print(roundup(0.50));  /* 1となる */
print(roundup(-0.50)); /* 0となる */</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/arithmetic/round">round</a>, <a href="/method/arithmetic/rounddown">rounddown</a>, <a href="/method/arithmetic/roundm">roundm</a> methods</td>
  </tr>
</table>





