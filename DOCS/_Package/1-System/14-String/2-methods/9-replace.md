---
layout: default

grand_parent: String Class
parent: Properties
has_children: false
title: String.Replace Method
nav_order: 9
permalink: /package/system/string/methods/replace
---
# {{ page.title }}
 
<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Finds the specified string and replaces everything found with another string.<br><br>This method updates the value of the String object.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = str.Replace( <b>search</b>, <b>replace</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Character string as a result of replacement</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>search</b></td>
    <td>Search string</td>
  </tr>
  <tr>
    <td>String <b>replace</b></td>
    <td>String to replace</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new String("abcdefg");
print(str.Replace("cde", "CDE"), "\n");
print(str, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>