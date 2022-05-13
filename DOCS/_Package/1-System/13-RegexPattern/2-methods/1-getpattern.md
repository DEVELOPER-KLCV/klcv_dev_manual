---
layout: default

grand_parent: RegexPattern Class
parent: Methods
has_children: false
title: RegexPattern.GetPattern Method
nav_order: 1
permalink: /package/system/regexpattern/methods/getpattern
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the string of the regular expression from which it was compiled.<br> <small>Added since Ver.5.0.1</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var pattern = rp.GetPattern( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Regular expression string from the compile source<br> In <a href="/package/system/regexpattern/#about-unicode-mode">Unicode mode</a>, it returns as UString type, otherwise it returns as String type.</td>
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
var p = RegexPattern.Compile("Biz/([a-zA-Z]+)", 0, RegexPattern.Unicode);
print(p.GetPattern(), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexpattern/properties/pattern">Pattern</a> property<br><a href="/package/system/regexpattern/methods/compile">Compile</a> method</td>
  </tr>
</table>
