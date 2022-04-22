---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.Group Method
nav_order: 6
permalink: /package/system/regexmatcher/methods/group
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = rm.Group( [ <b>group</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>group</b></td>
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
var m = RegexPattern.Compile("Biz/([a-zA-Z]+)").Matcher("Biz/Browser");
if (m.Matches()) {
    print(m.Start(1), m.End(1), m.Group(1), "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexmatcher/methods/start">Start</a>, <a href="/package/system/regexmatcher/methods/end">End</a> methods</td>
  </tr>
</table>
