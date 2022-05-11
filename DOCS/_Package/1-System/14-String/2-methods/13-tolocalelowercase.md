---
layout: default

grand_parent: String Class
parent: Properties
has_children: false
title: String.ToLocaleLowerCase Method
nav_order: 13
permalink: /package/system/string/methods/tolocalelowercase
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Converts uppercase letters in strings to lowercase letters based on the locale.<br>In the current implementation, it is synonymous with the <a href="/package/system/string/methods/tolowercase">ToLowerCase</a> method.<br><br>This method updates the value of the String object.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = str.ToLocaleLowerCase( )</td>
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
var str = new String("abcdEFGH");
print(str.ToLocaleLowerCase(), "\n");
print(str, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/string/methods/tolowercase">ToLowerCase</a> method</td>
  </tr>
</table>