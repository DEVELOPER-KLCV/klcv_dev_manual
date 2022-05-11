---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.Reset Method
nav_order: 11
permalink: /package/system/regexmatcher/methods/reset
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Reset the regular expression engine.<br><br>Resetting the regular expression engine initializes the current position of the <a href="/package/system/regexmatcher/methods/find">Find</a> method, the additional position of the <a href="/package/system/regexmatcher/methods/appendreplacement">Appendreplacement</a> method, the match information that can be obtained using the <a href="/package/system/regexmatcher/methods/start">Start</a>, <a href="/package/system/regexmatcher/methods/end">End</a>, <a href="/package/system/regexmatcher/methods/group">Group</a> methods, and so on.<br><br>You can also set a new input string by specifying input.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = rm.Reset( [ input ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Own RegexMatcher object</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>input</b></td>
    <td>Newly set input string<br>If omitted, the input string will not be changed.<br><small>From Ver.5.0.1, it is treated as UString type in Unicode mode.</small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var m = RegexPattern.Compile("(Biz)/([a-zA-Z]+)").Matcher("Biz/Browser, PrintStream");
while (m.Find()) {
    print(m.Group(1), m.Group(2), "\n");
}
m.Reset("Biz/Browser, Biz/Designer");
print("----Reset----\n");
while (m.Find()) {
    print(m.Group(1), m.Group(2), "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>
