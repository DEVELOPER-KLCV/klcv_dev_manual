---
layout: default

grand_parent: Date Class
parent: Methods
has_children: false
title: Date.SetMilliSeconds Method
nav_order: 27
permalink: /package/system/date/methods/SetMilliSeconds
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the millisecond part in local time.<br>Although defined for compatibility with JavaScript , the resolution of the Date class is 1 second, so the value does not change when this method is executed.</td>
  </tr>
 　<tr>
    <td>Call format</td>
    <td colspan="2">d.SetMilliSeconds (<b><i>value</i></b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer  <b><i>ms</i></b></td>
    <td>Specify the millisecond.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = new Date ();
d.SetMilliSeconds (0);
print (d, "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>