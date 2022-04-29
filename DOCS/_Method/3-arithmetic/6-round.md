---
layout: default

parent: 3. Arithmetic Functions

title: round
nav_order: 6
permalink: /method/arithmetic/round
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Rounds to the specified digit.<br>If the number of digits is omitted, the number after the decimal point is rounded off.<br><br>Rounding of the round function (when the number of digits = 0) will be <b>Value + the maximum (positive direction) of integers less than or equal to 0.5</b><br><br>*<small>Added since Version 2.0.0</small>*</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var r = round( <b>arg</b>, <b>n</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns the value rounded to the specified number of digits.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Number <b>arg</b></td>
    <td>Original number</td>
  </tr>
  <tr>
    <td>Number <b>n</b></td>
    <td>Position of the digit to be rounded</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>print(round(12345.678, -2)); /* 12300となる */
print(round(12345.678));     /* 12346となる */
print(round(12345.678, 2));  /* 12345.68となる */
 
print(round(0.49));  /* 0となる */
print(round(0.50));  /* 1となる */
print(round(0.51));  /* 1となる */
print(round(-0.49)); /* 0となる */
print(round(-0.50)); /* 0となる */
print(round(-0.51)); /* -1となる */</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/arithmetic/rounddown">rounddown</a>, <a href="/method/arithmetic/roundup">roundup</a>, <a href="/method/arithmetic/roundm">roundm</a> methods</td>
  </tr>
</table>





