---
layout: default

parent: Date Functions

title: day
nav_order: 3
permalink: /method/date/day
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the day value of a date represented by <b>date</b>.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var d = day( <b>date</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a number from 1 to 31 that represents the 1st to 31st.<br>Otherwise it will be 0.</td>
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
var t = day(d);</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/date/year">year</a>, <a href="/method/date/month">month</a>, <a href="/method/date/youbi">youbi</a> methods </td>
  </tr>
</table>





