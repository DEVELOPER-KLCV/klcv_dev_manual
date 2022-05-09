---
layout: default

grand_parent: Number Class
parent: Methods
has_children: false
title: Number.ToString Method
nav_order: 6
permalink: /package/system/number/methods/tostring
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the value stored in the Number object as a string.<br>Returns as a <b>radix</b> base string by specifying an argument</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var text = num.ToString( [ <b>radix</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Converted string</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>radix</b></td>
    <td>radix<br>Can specify a value between 2 and 36. Specify 16 for hexadecimal numbers.<br>Default is decimal.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>The argument value is invalid.</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var num = new Number;
num.Value = 5678;
print(num.ToString(16), "\n");
 
---Output result---
162e</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



