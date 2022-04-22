---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.Find Method
nav_order: 4
permalink: /package/system/regexmatcher/methods/find
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var b = rm.Find( [ <b>start</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>start</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func 4</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var m = RegexPattern.Compile("Biz").Matcher("Biz/Browser, Biz/Desginer, Biz-Collections");
while (m.Find()) {
    print(m.Start(0), m.End(0), "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexmatcher/methods/start">Start</a>, <a href="/package/system/regexmatcher/methods/end">End</a>, <a href="/package/system/regexmatcher/methods/group">Group</a>, <a href="/package/system/regexmatcher/methods/reset">Reset</a> methods</td>
  </tr>
</table>
