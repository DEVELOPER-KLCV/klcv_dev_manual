---
layout: default

grand_parent: UString Class
parent: Properties
has_children: false
title: UString.CharAt Method
nav_order: 2
permalink: /package/system/ustring/methods/charat
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the character at the specified position.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var n = str.CharAt( <b>indx</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns one character at the specified position as a UString type.</td>
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
var str = new UString("ABCDEF");
print(str.CharAt(3), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/ustring/methods/charcodeat">CharCodeAt</a> method</td>
  </tr>
</table>