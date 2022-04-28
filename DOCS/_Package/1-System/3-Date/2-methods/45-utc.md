---
layout: default

grand_parent: Date Class
parent: Methods
has_children: false
title: Date.UTC Method
nav_order: 45
permalink: /package/system/date/methods/utc
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the elapsed time from the UTC reference time for the specified date in milliseconds.<br>This method is a static method.It can be called without creating an object.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var v = Date.UTC (<b><i>year , month , date [, hour [, min [, sec [, ms ]]]]</i></b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns the elapsed time in milliseconds since the UTC reference time.</td>
  </tr>  
  <tr>
    <td rowspan="7">Arguments</td>
    <td>integer <b><i>year</i></b></td>
    <td>Specify the year in UTC time.</td>
  </tr>  
  <tr>
    <td>integer <b><i>month</i></b></td>
    <td>Specify the month number with January as 0.</td>
  </tr>   
  <tr>
    <td>integer <b><i>date</i></b></td>
    <td>Specify the day in UTC time.</td>
  </tr>   
  <tr>
    <td>integer <b><i>hour</i></b></td>
    <td>Specify the time in UTC time.</td>
  </tr>   
  <tr>
    <td>integer <b><i>min</i></b></td>
    <td>Specify the minutes in UTC time.</td>
  </tr>   
  <tr>
    <td>integer <b><i>sec</i></b></td>
    <td>Specifies seconds in UTC time.</td>
  </tr>   
  <tr>
    <td>integer <b><i>ms</i></b></td>
    <td>Ignored.</td>
  </tr>    
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = new Date ();
d.SetTime (Date.UTC (2002, 2, 28, 20, 0, 0));
print (d, "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>

