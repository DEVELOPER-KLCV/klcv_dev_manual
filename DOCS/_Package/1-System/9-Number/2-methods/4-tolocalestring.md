---
layout: default

grand_parent: Number Class
parent: Methods
has_children: false
title: Number.ToLocaleString Method
nav_order: 4
permalink: /package/system/number/methods/tolocalestring
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the value stored in the Number object as a locale-formatted string. <br>The current implementation returns the same value as the <a href="/package/system/number/methods/tostring">ToString</a> method.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var text = num.ToLocaleString( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Locale format string</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var num = new Number;
num.Value = 5678;
print(num.ToLocaleString(), "￥n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/number/methods/tostring">ToString</a> method</td>
  </tr>
</table>



