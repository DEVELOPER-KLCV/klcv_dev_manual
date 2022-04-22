---
layout: default

grand_parent: RegexPattern Class
parent: Methods
has_children: false
title: RegexPattern.Compile Method
nav_order: 4
permalink: /package/system/regexpattern/methods/compile
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var rp = RegexPattern.Compile( <b>regex</b> [, <b>flags</b> [, <b>mode</b> ]] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">RegexPattern object</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>String <b>regex</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>flags</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>mode</b></td>
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
var p = RegexPattern.Compile("Biz/([a-zA-Z]+)", RegexPattern.CASELESS, RegexPattern.Unicode);
var m = p.Matcher("Biz/Browser");
if (m.Matches()) {
    print(m.Group(1), "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexpattern/methods/matches">Matches</a> method</td>
  </tr>
</table>
