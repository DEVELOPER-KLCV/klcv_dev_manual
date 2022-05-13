---
layout: default

grand_parent: String Class
parent: Methods
has_children: false
title: String.IndexOf Method
nav_order: 6
permalink: /package/system/string/methods/indexof
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Finds the specified string after <b>pos</b> and returns the first found position.<br><br>This method finds without being aware of the character type of the target character string. Use the <a href="/method/str/find">Find</a> function to search for double-byte characters in the target string</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var n = str.IndexOf( <b>find</b> [, <b>pos</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a zero -based number that indicates the location found. Returns -1 if not found</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>find</b></td>
    <td>Character string to find</td>
  </tr>
  <tr>
    <td>integer <b>pos</b></td>
    <td>Search range start position<br>Specify a number starting from 0 . If omitted, the search starts from the beginning.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">Invalid argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str1 = new String("abcdefg abcdefg");
print(str1.IndexOf("cd"), "\n");
 
 
/* When the target character string contains double-byte characters */
var str2 = new String("東京都千代田区千代田1番1号");
print(find(str2, "1", 0), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/string/methods/lastindexof">LastIndexOf</a>method<br><a href="/method/str/find">Find</a> method</td>
  </tr>
</table>