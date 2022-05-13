---
layout: default

grand_parent: Date Class
parent: Methods
has_children: false
title: Date.SetUTCFullYear Method
nav_order: 28
permalink: /package/system/date/methods/setutcfullyear
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the year part in UTC time.<br>The omitted parameter items are not changed.</td>
  </tr>
 　<tr>
    <td>Call format</td>
    <td colspan="2">d.SetUTCFullYear  (<b><i>value [, mon [, date ]]</i></b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer  <b><i>value</i></b></td>
    <td>Specify the year numerically.</td>
  </tr>
    <tr>
    <td>integer  <b><i>mon</i></b></td>
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
d.SetUTCFullYear (2000);
print (d, "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>