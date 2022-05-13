---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.AppendTail Method
nav_order: 2
permalink: /package/system/regexmatcher/methods/appendtail
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td>Behaves as a append-and-replace method.<br><br> Returns from the input string after appends it at the tail position.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td>var s = rm.AppendTail( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td>Character string from the input character string after the append position to the tail.<br><small>From Ver.5.0.1, UString type character string is returned in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>.</small></td>
  </tr>  
  <tr>
    <td>Argument</td>
    <td>None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td><code><pre>
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
    <td><a href="/package/system/regexmatcher/methods/appendreplacement">AppendReplacement</a> method</td>
  </tr>
</table>
