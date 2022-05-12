---
layout: default

grand_parent: Date Class
parent: Methods
has_children: false
title: Date.SetUTCMinutes Method
nav_order: 32
permalink: /package/system/date/methods/setutcminutes
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the minute part in UTC time.<br>The omitted parameter items are not changed.</td>
  </tr>
 　<tr>
    <td>Call format</td>
    <td colspan="2">d.SetUTCMinutes (<b><i>value [, sec [, ms ]]]</i></b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer  <b><i>value</i></b></td>
    <td>Specify the minute numerically.</td>
  </tr>
  <tr>
    <td>integer  <b><i>sec</i></b></td>
    <td>Specify the seconds numerically.</td>
  </tr>
  <tr>
    <td>integer <b><i>ms</i></b></td>
    <td>Specify the millisecond. The resolution accuracy of the Date class is 1 second, so even if you specify <b><i>ms</i></b>, it does not affect the result</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = new Date ();
print (d, "￥ n");
d.SetUTCMinutes (0);
print (d, "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>