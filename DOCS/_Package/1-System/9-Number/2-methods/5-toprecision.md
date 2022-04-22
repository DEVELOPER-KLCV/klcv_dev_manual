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
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var text = num.ToPrecision( [ <b>fractionDigits</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>fractionDigits</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var num = new Number;
num.Value = 5678.12345;
print(num.ToPrecision(3), "\n");
print(num.ToPrecision(6), "\n");
 
---出力結果---
5.68e+003
5678.12</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/number/methods/toexponential">ToExponential</a>, <a href="/package/system/number/methods/tofixed">ToFixed</a>, <a href="/package/system/number/methods/tostring">ToString</a> method</td>
  </tr>
</table>



