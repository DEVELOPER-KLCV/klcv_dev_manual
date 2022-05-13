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
    <td colspan="2">Gets the substring of the matched result.<br><br>If you specify <b>group</b>, you can get the substring forward-referenced by the group of regular expression patterns. Groups are numbered from 1 to right, with group 0 representing the entire pattern.<br><br>Regular expression patterns such as "(a) *" may match the empty string. In this case, an empty string is returned.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = rm.Group( [ <b>group</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Matched part or substring of forward reference group<br><small>From Ver.5.0.1, UString type string is returned in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>.</small></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>group</b></td>
    <td>The number of the forward reference group you want to get<br>If omitted, it will be 0 (entire pattern).</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>Func 4</td>
    <td>The argument value is invalid</td>
  </tr>
  <tr>
    <td>Func 14</td>
    <td>The value cannot be referenced</td>
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
