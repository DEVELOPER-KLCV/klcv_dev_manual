---
layout: default

grand_parent: RegexPattern Class
parent: Methods
has_children: false
title: RegexPattern.Matcher Method
nav_order: 2
permalink: /package/system/regexpattern/methods/matcher
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Creates a RegexMatcher object that matches the regular expression pattern with the input string.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var rm = rp.Matcher( <b>input</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">RegexMatcher object</td>
  </tr>
  <tr>
    <td>Arguments</td>
    <td>String <b>input</b></td>
    <td>Matching input string<br><small>From Ver.5.0.1, it is treated as UString type in <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>.</small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var p = RegexPattern.Compile("Biz/([a-zA-Z]+)");
    var m = p.Matcher("Biz/Browser");
    if (m.Matches()) {
        print(m.Group(1), "\n");
    }
    </pre></code></td>
  </tr>
  
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexmatcher">RegexMatcher</a> class</td>
  </tr>
</table>
