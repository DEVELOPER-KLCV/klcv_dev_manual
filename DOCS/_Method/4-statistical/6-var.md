---
layout: default

parent: Statistical Functions

title: var
nav_order: 6
permalink: /method/statistical/var
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Consider the data as the entire population and find its variance.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var v = var  ( <b>range</b> )</td>
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
print (var (arr), "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/statistical/vars">vars</a> function</td>
  </tr>
</table>





