---
layout: default

grand_parent: Number Class
parent: Methods
has_children: false
title: Number.ToPrecision Method
nav_order: 5
permalink: /package/system/number/methods/toprecision
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the value stored in the Number object as a string in exponential or fixed-point notation for the specified number of digits.<br>If the argument is omitted, the result equivalent to the <a href="/package/system/number/methods/tostring">ToString</a> method is returned.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var text = num.ToPrecision( [ <b>fractionDigits</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">String in exponential or fixed-point notation. <br>Returns the one with the shorter expression.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>fractionDigits</b></td>
    <td>Number of digits. <br>Specify 1 to 15.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>The argument value is invalid</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var num = new Number;
num.Value = 5678.12345;
print(num.ToPrecision(3), "￥n");
print(num.ToPrecision(6), "￥n");
 
---Output result---
5.68e+003
5678.12</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/number/methods/toexponential">ToExponential</a>, <a href="/package/system/number/methods/tofixed">ToFixed</a>, <a href="/package/system/number/methods/tostring">ToString</a> method</td>
  </tr>
</table>



