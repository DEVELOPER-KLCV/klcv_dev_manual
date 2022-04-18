---
layout: default

parent: Date Functions

title: youbi
nav_order: 9
permalink: /method/date/youbi
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the day number of the date represented by <b>date</b>.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var d = youbi( <b>date</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">The day numbers are as follows.<br>0: Mon 1: Tue 2: Wed 3: Thu 4: Fri 5: Sat 6: Sun</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Date <b>date</b></td>
    <td>Date object to retrieve the day of the week</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = sysdate();
var w = youbi(d);</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/date/year">year</a>, <a href="/method/date/month">month</a>, <a href="/method/date/day">day</a> methods </td>
  </tr>
</table>









