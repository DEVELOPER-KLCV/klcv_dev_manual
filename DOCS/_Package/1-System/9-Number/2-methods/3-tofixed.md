---
layout: default

grand_parent: Number Class
parent: Methods
has_children: false
title: Number.ToFixed Method
nav_order: 3
permalink: /package/system/number/methods/tofixed
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the value stored in the Number object as a fixed-point string.<br>*Use the <a href="/package/system/fixed/methods/constructor">Fixed constructor</a> to convert to the Fixed class.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var text = num.ToFixed( [ <b>fractionDigits</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Fixed-point notation string</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>fractionDigits</b></td>
    <td>Number of digits after the decimal point. <br>It can be specified between 0 and 15. If omitted, it will be 0.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>The argument value is invalid.</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var num = new Number;
num.Value = 5678.12345;
print(num.ToFixed(3), "\n");
 
---Output result---
5678.123</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



