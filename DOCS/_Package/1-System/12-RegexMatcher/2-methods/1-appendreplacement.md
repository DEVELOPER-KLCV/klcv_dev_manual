---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.AppendReplacement Method
nav_order: 1
permalink: /package/system/regexmatcher/methods/appendreplacement
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Performs continuous append and replacement.<br><br>Returns the character string from the input character string after the append position to the previously matched part. At this time, the matched part is replaced with the replacement character string. The append position then moves to the next position in the trailing index of the match.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = rm.AppendReplacement( <b>replacement</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">From the input character string after the append position to the part that matched last time, the match part is replaced with the replacement character string and returned.<br><small>From Ver.5.0.1, UString type character string is returned in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>.</small></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>replacement</b></td>
    <td>Replacement string<br>You can use a <a href="/package/system/regexmatcher">reference to a forward reference group by "$ n"</a> <br><small>From Ver.5.0.1, it is treated as UString type in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>.</small></td>
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
    <td colspan="2"><a href="/package/system/regexmatcher/methods/appendtail">AppendTail</a> method</td>
  </tr>
</table>
