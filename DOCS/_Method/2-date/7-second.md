---
layout: default

parent: 2. Date Functions

title: second
nav_order: 7
permalink: /method/date/second
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the second value of the time represented by <b>date</b>.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var d = second( <b>date</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a number from 0 to 59 that represents 0 to 59 seconds.<br>Otherwise it will be 0.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Date <b>date</b></td>
    <td>Date object to retrieve the seconds</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = sysdate();
var s = second(d);</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/date/hour">hour</a>, <a href="/method/date/minute">minute</a> methods </td>
  </tr>
</table>









