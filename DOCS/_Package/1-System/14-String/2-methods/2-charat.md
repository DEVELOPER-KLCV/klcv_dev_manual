---
layout: default

grand_parent: String Class
parent: Properties
has_children: false
title: String.CharAt Method
nav_order: 2
permalink: /package/system/string/methods/charat
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the character at the specified byte position.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var n = str.CharAt( <b>indx</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns one character at the specified position as a String type.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>indx</b></td>
    <td>Position of the character to be extracted<br>Specify a number starting from 0.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new String("ABCDEF");
print(str.CharAt(3), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/string/methods/charcodeat">CharCodeAt</a> method</td>
  </tr>
</table>