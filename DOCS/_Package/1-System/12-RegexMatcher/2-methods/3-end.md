---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.End Method
nav_order: 3
permalink: /package/system/regexmatcher/methods/end
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the tail index of the matched result.<br><br>Able to  specify <b>group</b> to get the tail index of a substring forward-referenced by a group of regular expression patterns.<br>Groups are numbered from left to right, starting with 1 , and group 0 represents the entire pattern.<br><br>Regular expression patterns such as "(a) *" may match the empty string. In this case it returns -1. However, if you specify 0 for the group number, 0 is returned.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var e = rm.End( [ <b>group</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">End index of matched part or forward reference group.<br>(The tail index points to the next position at the end of the string).<br><small>From Ver.5.0.1, the index is in character units in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>.Other than that, it is in bytes.</small></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>group</b></td>
    <td>The number of the forward reference group you want to get.<br>If omitted, it will be 0 (entire pattern).</td>
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
    <td colspan="2"><a href="/package/system/regexmatcher/methods/start">Start</a>, <a href="/package/system/regexmatcher/methods/group">Group</a> methods</td>
  </tr>
</table>
