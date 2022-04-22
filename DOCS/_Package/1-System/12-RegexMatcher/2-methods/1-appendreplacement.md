---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.AppendReplacement Method
nav_order: 1
permalink: /package/system/regexmatcher/methods/appendreplacement
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = rm.AppendReplacement( <b>replacement</b> )</td>
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
    <td rowspan="2">Exception</td>
    <td>Func 4</td>
    <td></td>
  </tr>
  <tr>
    <td>Func 14</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var p = RegexPattern.Compile("([0-9])([0-9])([0-9])");
var m = p.Matcher("Biz/Browser 311, Biz/Desginer 400, abcde");
var s = "";
while (m.Find()) {
    s += m.AppendReplacement("$1.$2.$3");
}
s += m.AppendTail();
print(s, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexmatcher/methods/appendtail">AppendTail</a> method</td>
  </tr>
</table>
