---
layout: default

grand_parent: String Class
parent: Properties
has_children: false
title: String.Split Method
nav_order: 11
permalink: /package/system/string/methods/split
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var arr = str.Split( <b>separator</b> [, <b>limit</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>separator</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>limit</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new String("abc-def-ghi");
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