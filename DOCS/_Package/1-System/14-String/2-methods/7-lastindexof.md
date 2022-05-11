---
layout: default

grand_parent: String Class
parent: Properties
has_children: false
title: String.LastIndexOf Method
nav_order: 7
permalink: /package/system/string/methods/lastindexof
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Searches the specified string up to <b>pos</b> and returns the last found position.<br><br>This method searches without being aware of the character type of the target character string. Use the find function to search for double-byte characters in the target string</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var n = str.LastIndexOf( <b>find</b> [, <b>pos</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a zero -based number that indicates the location found. Returns -1 if not found</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>find</b></td>
    <td>Character string to search</td>
  </tr>
  <tr>
    <td>integer <b>pos</b></td>
    <td>End position of search range<br>Specify a number starting from 0. If omitted, the search will be performed to the end.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str1 = new String("abcdefg abcdefg");
print(str1.LastIndexOf("cd"), "\n");
 
 
/* When the target character string contains double-byte characters */
var str2 = new String("東京都千代田区千代田1番1号");
var last = -1;
while (true) {
    var idx = find(str2, "1", last + 1);
    if (idx < 0) {
        break;
    }
    last = idx;
}
print(last, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/string/methods/indexof">IndexOf</a> method<br><a href="">find</a> method</td>
  </tr>
</table>