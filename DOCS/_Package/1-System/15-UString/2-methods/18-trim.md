---
layout: default

grand_parent: UString Class
parent: Methods
has_children: false
title: UString.Trim Method
nav_order: 18
permalink: /package/system/ustring/methods/trim
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Remove spaces, tabs, line breaks, etc. from the front and back of the string.<br><br>The target character can be specified to be removed by specifying an argument.If the argument is omitted, tabs, single-byte spaces, and line breaks are targeted. (Full-width space is not applicable)<br>Unlike the <a href="/method/str/trim">trim</a> function, it does not change anything other than before and after the string.<br><br>This method updates the value of the String object.<br><br><small>Added since Ver.5.0.0<br>Not available on Mobile</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = str.Trim( [ <b>chars</b> ])</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Character string with spaces removed</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>UString <b>chars</b></td>
    <td>Characters to be removed<br>Specify the character string in which the characters you want to remove are arranged.<br>If omitted, tabs, half-width spaces, and line breaks are targeted.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new String(" ABC\tDEF\n ");
print(str.Trim(" \t\n　"), "\n");
print(str, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/str/trim">trim</a> method</td>
  </tr>
</table>