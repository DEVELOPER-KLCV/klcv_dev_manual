---
layout: default

grand_parent: RegexMatcher Class
parent: Methods
has_children: false
title: RegexMatcher.ReplaceAll Method
nav_order: 9
permalink: /package/system/regexmatcher/methods/replaceall
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Replaces everything that matches the regular expression pattern with the specified string.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = rm.ReplaceAll( replacement )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Replaced result string<br><small>From Ver.5.0.1, UString type string is returned in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>.</small></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>replacement</b></td>
    <td>Replacement string<br>You can use a <a href="/package/system/regexmatcher/#about-the-reference-to-the-forward-reference-group-of-the-replace-operation-method">reference to a forward reference group by "$n"</a> <br><small>From Ver.5.0.1, it is treated as UString type in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>.</small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func 14</td>
    <td>The value cannot be referenced</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var p = RegexPattern.Compile("Biz/([a-zA-Z]+)");
var m = p.Matcher("Biz/Browser, Biz/Designer");
print(m.ReplaceAll("ABC Biz/$1"), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexmatcher/methods/replacefirst">ReplaceFirst</a> method</td>
  </tr>
</table>
