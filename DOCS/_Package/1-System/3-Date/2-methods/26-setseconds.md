---
layout: default

grand_parent: Date Class
parent: Methods
has_children: false
title: Date.SetSeconds Method
nav_order: 26
permalink: /package/system/date/methods/SetSeconds
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the seconds part in local time.<br>The omitted parameter items are not changed.</td>
  </tr>
 　<tr>
    <td>Call format</td>
    <td colspan="2">d.SetSeconds  (<b><i>value [, ms ]]]</i></b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer  <b><i>value</i></b></td>
    <td>Specify the seconds numerically.</td>
  </tr>
    <tr>
    <td>integer  <b><i>ms</i></b></td>
    <td>Specify the millisecond. The resolution accuracy of the Date class is 1 second, so even if you specify <b><i>ms</i></b>, it does not affect the result.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = new Date ();
print (d, "￥ n");
d.SetSeconds (0);
print (d, "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>