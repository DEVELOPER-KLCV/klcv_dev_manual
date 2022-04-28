---
layout: default

grand_parent: Date Class
parent: Methods
has_children: false
title: Date.SetUTCMonth Method
nav_order: 29
permalink: /package/system/date/methods/SetUTCMonth
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the month part in UTC time.<br>The omitted parameter items are not changed.</td>
  </tr>
 　<tr>
    <td>Call format</td>
    <td colspan="2">d.SetUTCMonth (<b><i>value [, date ]]</i></b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer  <b><i>value</i></b></td>
    <td>Specify the month as a month number with January as 0.</td>
  </tr>
    <tr>
    <td>integer  <b><i>date</i></b></td>
    <td>Specify the day numerically.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = new Date ();
print (d, "￥ n");
d.SetUTCMonth (10);
print (d, "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>