---
layout: default

grand_parent: UString Class
parent: Methods
has_children: false
title: UString.IndexOf Method
nav_order: 6
permalink: /package/system/ustring/methods/indexof
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Finds the specified string after <b>pos</b> and returns the first found position.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var n = str.IndexOf( <b>find</b> [, <b>pos</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a zero -based number that indicates the location found. Returns -1 if not found.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>UString <b>find</b></td>
    <td>Character string to search</td>
  </tr>
  <tr>
    <td>integer <b>pos</b></td>
    <td>Search range start position<br>Specify a number starting from 0 . If omitted, the search starts from the beginning.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new UString("abcdefg abcdefg");
print(str.IndexOf("cd"), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/ustring/methods/lastindexof">LastIndexOf</a> method</td>
  </tr>
</table>