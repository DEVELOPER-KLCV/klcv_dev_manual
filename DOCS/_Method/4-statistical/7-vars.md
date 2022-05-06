---
layout: default

parent: 4. Statistical Functions

title: vars
nav_order: 7
permalink: /method/statistical/vars
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Use the data as an extraction sample from the population to find the population variance.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var v = vars  ( <b>range</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Distribution of data within <b>range</b></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Date or Number <b>range</b></td>
    <td>Array object name</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var arr = new Number [20];
for (var n = 0; n <arr.Length; n ++) {
    arr [n] = int (rand () * 10);
    print (arr [n], "");
}
print (vars (arr), "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/statistical/var">var</a> function</td>
  </tr>
</table>




