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
    <td colspan="2">Searches the input string for the next substring that matches the regular expression pattern.<br><br>Immediately after generating the regular expression engine or reset by the <a href="/package/system/regexmatcher/methods/reset">Reset</a> method, the search starts from the beginning of the input string.<br><br>If no argument is specified, the search will start after the previous match.<br>The <b>start</b> argument resets the regular expression engine and starts the search at the specified position in <b>start</b> of the input string.<br><br>If the match is successful, you can use the <a href="/package/system/regexmatcher/methods/start">Start</a>, <a href="/package/system/regexmatcher/methods/end">End</a>, and <a href="/package/system/regexmatcher/methods/group">Group</a> methods to get more information.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var b = rm.Find( [ <b>start</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">$ TRUE if there is a partial match with the regular expression pattern after the current position of the input string, $ FALSE if not</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>start</b></td>
    <td>Search start position<br><small>From Ver.5.0.1, in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>, specify the start position in character units. Otherwise, specify in bytes.</small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func 4</td>
    <td>The argument value is invalid</td>
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
