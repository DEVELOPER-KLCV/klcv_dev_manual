---
layout: default

grand_parent: RegexPattern Class
parent: Methods
has_children: false
title: RegexPattern.Matches Method
nav_order: 5
permalink: /package/system/regexpattern/methods/matches
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var b = RegexPattern.Matches( <b>regex</b>, <b>input</b> [, <b>flags</b> [, <b>mode</b> ]] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">RegexPattern object</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>String <b>regex</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>input</b></td>
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
if (RegexPattern.Matches("[0-9]+/[0-9]+/[0-9]+", "2011/11/28")) {
    //.MessageBox("Matched");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/regexpattern/methods/compile">Compile</a>, <a href="/package/system/regexpattern/methods/matcher">Matcher</a> method</td>
  </tr>
</table>
