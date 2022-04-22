---
layout: default

grand_parent: RegexPattern Class
parent: Methods
has_children: false
title: RegexPattern.Split Method
nav_order: 3
permalink: /package/system/regexpattern/methods/split
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var arr = rp.Split( <b>input</b> [, <b>limit</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">RegexMatcher object</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>input</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>limit</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var p = RegexPattern.Compile("/");
var arr = p.Split("Biz/Browser");
for (var i = 0; i < arr.length; i++) {
    print(arr[i], "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>
