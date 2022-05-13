---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.GetInputString Method
nav_order: 5
permalink: /package/system/regexmatcher/methods/getinputstring
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td>Gets the input string set in the regular expression engine.<br><small>Added since Ver.5.0.1</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td>var s = rm.GetInputString( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td>Input string set in the regular expression engine<br>In <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>, it returns as UString type, otherwise it returns as String type.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var p = RegexPattern.Compile("Biz/([a-zA-Z]+)", 0, RegexPattern.Unicode);
var m = p.Matcher("Biz/Browser,Biz/Designer");
print(m.GetInputString(), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexmatcher/properties/inputstring">InputString</a> property</td>
  </tr>
</table>
