---
layout: default

grand_parent: String Class
parent: Properties
has_children: false
title: String.EqualsIgnoreCase Method
nav_order: 5
permalink: /package/system/string/methods/equalsignorecase
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = str.EqualsIgnoreCase( s )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>s</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new String("ABC");
var arr = new Array("ABC", "abc", "xyz");
for (var n in arr) {
    if (str.EqualsIgnoreCase(arr[n])) {
        print(arr[n], "\n");
    }
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/string/methods/localecompare">LocaleCompare</a> method</td>
  </tr>
</table>