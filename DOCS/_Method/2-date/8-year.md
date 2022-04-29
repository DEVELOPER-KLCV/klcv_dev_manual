---
layout: default

parent: 2. Date Functions

title: year
nav_order: 8
permalink: /method/date/year
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the year value of a date represented by <b>date</b>.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var d = year( <b>date</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a number representing the year between 1900 and 2099.<br>Otherwise it will be 0.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Date <b>date</b></td>
    <td>Date object to retrieve the year</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = sysdate();
var y = year(d);</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/date/month">month</a>, <a href="/method/date/day">day</a>, <a href="/method/date/youbi">youbi</a> methods </td>
  </tr>
</table>









