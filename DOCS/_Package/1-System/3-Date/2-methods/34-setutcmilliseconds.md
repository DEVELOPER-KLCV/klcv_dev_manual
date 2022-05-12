---
layout: default

grand_parent: Date Class
parent: Methods
has_children: false
title: Date.SetUTCMilliSeconds Method
nav_order: 34
permalink: /package/system/date/methods/setutcmilliseconds
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the millisecond part in UTC time.<br>Although defined for compatibility with JavaScript , the resolution of the Date class is 1 second, so the value does not change when this method is executed.</td>
  </tr>
 　<tr>
    <td>Call format</td>
    <td colspan="2">d.SetUTCMilliSeconds  (<b><i>value</i></b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b><i>value</i></b></td>
    <td>Specify the number of milliseconds.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = new Date ();
d.SetUTCMilliSeconds  (0);
print (d, "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>