---
layout: default

parent: 2. Date Functions

title: datedif
nav_order: 1
permalink: /method/date/datedif
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the period from the <b>start date</b> to the <b>end date</b>.<br>The start and end date times are ignored.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var y = datedif (<b>start date</b>, <b>end date</b>, <b>output specification</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns the difference between the <b>end date</b> and the <b>start date</b> with the specified <b>output specification</b>.</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>Date <b>Start date</b></td>
    <td>Start date</td>
  </tr>
  <tr>
    <td>Date <b>End date</b></td>
    <td>End date</td>
  </tr>
  <tr>
    <td>String <b>output specification</b></td>
    <td>"y" years elapsed<br>"m" Number of months elapsed<br>"d" Elapsed days<br>"md" Fraction of days less than a month<br>"ym" Fraction of months less than a year<br>"yd" Fraction of days less than a year</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d1 = dateval("1964/8/10");
var d2 = sysdate();
var s = datedif(d1, d2, "y");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>





