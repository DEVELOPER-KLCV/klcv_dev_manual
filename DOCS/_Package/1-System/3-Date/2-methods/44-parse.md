---
layout: default

grand_parent: Date Class
parent: Methods
has_children: false
title: Date.Parse Method
nav_order: 44
permalink: /package/system/date/methods/parse
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Parses the date string.This method is a static method. It can be called without creating an object.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var v = Date.Parse (<b><i>value</i></b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns the elapsed time in milliseconds since the UTC reference time , which represents the date and time parsed.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String   <b><i>value</i></b></td>
    <td>Specifies a string that indicates the date and time.<br>The formats that can be parsed are as follows.<br>"YY / MM / DD"<br>"YY / MM / DD HH24: MI"<br>"YY / MM / DD HH24: MI: SS"<br>"YYYY / MM / DD"<br>"YYYY / MM / DD HH24: MI"<br>"YYYY / MM / DD HH24: MI: SS"<br>"dy, DD mon YYYY HH24: MI: SS TZ"</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = new Date ();
d.SetTime (Date.Parse ("2002/2/28 20:00:00"));
print (d, "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>

