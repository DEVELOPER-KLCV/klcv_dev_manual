---
layout: default

grand_parent: UString Class
parent: Properties
has_children: false
title: UString.Split Method
nav_order: 11
permalink: /package/system/ustring/methods/split
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Divides the string by the specified characters and returns it as an array.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var arr = str.Split( <b>separator</b> [, <b>limit</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">String array containing each element of the split string (does not include the delimiter)</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>UString <b>separator</b></td>
    <td>Delimiter to split a string</td>
  </tr>
  <tr>
    <td>integer <b>limit</b></td>
    <td>Maximum number to divide<br>If omitted, it will be split up to the end of the character string.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new UString("abc-def-ghi");
var arr = str.Split("-");
for (var n = 0; n < arr.Length; n++) {
    print(arr[n], "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>