---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.LookingAt Method
nav_order: 7
permalink: /package/system/regexmatcher/methods/lookingat
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var b = rm.LookingAt( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var m = RegexPattern.Compile("Biz/([a-zA-Z])+").Matcher("Biz/Browser, Biz/Desginer");
if (m.LookingAt()) {
    print(m.Start(1), m.End(1), m.Group(1), "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexmatcher/methods/start">Start</a>, <a href="/package/system/regexmatcher/methods/end">End</a>, <a href="/package/system/regexmatcher/methods/group">Group</a> methods</td>
  </tr>
</table>
