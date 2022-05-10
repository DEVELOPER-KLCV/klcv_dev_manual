---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.Matches Method
nav_order: 8
permalink: /package/system/regexmatcher/methods/matches
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Matches the entire input string with the regular expression pattern.<br><br>If the match is successful, you can use the <a href="/package/system/regexmatcher/methods/start">Start</a>, <a href="/package/system/regexmatcher/methods/end">End</a>, <a href="/package/system/regexmatcher/methods/group">Group</a> methods to get more information.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var b = rm.Matches( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">$ TRUE if the entire input string and the regular expression pattern match exactly, $ FALSE if not</td>
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
var m = RegexPattern.Compile("Biz/([a-zA-Z]+)").Matcher("Biz/Browser");
if (m.Matches()) {
    print(m.Start(1), m.End(1), m.Group(1), "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexmatcher/methods/start">Start</a>, <a href="/package/system/regexmatcher/methods/end">End</a>, <a href="/package/system/regexmatcher/methods/group">Group</a> methods</td>
  </tr>
</table>
