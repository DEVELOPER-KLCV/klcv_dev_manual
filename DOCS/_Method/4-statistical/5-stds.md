---
layout: default

parent: 4. Statistical Functions

title: stds
nav_order: 5
permalink: /method/statistical/stds
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Use the data as a sample extracted from the population to find the standard deviation of the population.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = stds ( <b>range</b> )</td>
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
print (stds  (arr), "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/statistical/std">std</a> function</td>
  </tr>
</table>




