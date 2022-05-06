---
layout: default

parent: 4. Statistical Functions

title: std
nav_order: 4
permalink: /method/statistical/std
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Consider the data as the entire population and find its standard deviation.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = std ( <b>range</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Standard deviation of data within <b>range</b></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Number <b>range</b></td>
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
print (std  (arr), "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/statistical/stds">stds</a> function</td>
  </tr>
</table>




