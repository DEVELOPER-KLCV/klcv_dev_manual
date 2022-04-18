---
layout: default

parent: Date Functions

title: hour
nav_order: 4
permalink: /method/date/hour
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the time value of the time represented by <b>date</b>.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var d = hour( <b>date</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a number from 0 to 23 that represents midnight to 23:00.<br>Otherwise it will be 0.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Date <b>date</b></td>
    <td>Date object to retrieve the day</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = sysdate();
var h = hour(d);</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/date/minute">minute</a>, <a href="/method/date/second">second</a> methods </td>
  </tr>
</table>





