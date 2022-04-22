---
layout: default

grand_parent: UString Class
parent: Properties
has_children: false
title: UString.Substring Method
nav_order: 12
permalink: /package/system/ustring/methods/substring
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = str.Substring( <b>start</b>, <b>end</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>start</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>end</b></td>
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
var str = new UString("abcdefghi");
print(str.Substring(1, 2), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/ustring/methods/slice">Slice</a> method</td>
  </tr>
</table>