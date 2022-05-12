---
layout: default

grand_parent: UString Class
parent: Properties
has_children: false
title: UString.ToLocaleUpperCase Method
nav_order: 14
permalink: /package/system/ustring/methods/tolocaleuppercase
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Converts lowercase letters in strings to uppercase based on the locale.<br>In the current implementation, it is synonymous with the <a href="/package/system/ustring/methods/touppercase">ToUpperCase</a> method<br><br>This method updates the value of the String object.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = str.ToLocaleUpperCase( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Converted string</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new UString("abcdEFGH");
print(str.ToLocaleUpperCase(), "\n");
print(str, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/ustring/methods/touppercase">ToUpperCase</a> method</td>
  </tr>
</table>