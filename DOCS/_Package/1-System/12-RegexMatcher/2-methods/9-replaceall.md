---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.ReplaceAll Method
nav_order: 9
permalink: /package/system/regexmatcher/methods/replaceall
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = rm.ReplaceAll( replacement )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>replacement</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func 14</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var p = RegexPattern.Compile("Biz/([a-zA-Z]+)");
var m = p.Matcher("Biz/Browser, Biz/Designer");
print(m.ReplaceAll("ABC Biz/$1"), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexmatcher/methods/replacefirst">ReplaceFirst</a> method</td>
  </tr>
</table>
